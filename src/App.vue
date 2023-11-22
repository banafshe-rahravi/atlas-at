<template>
  <div class="container">
    <ul class="content">
      <li class="content-1">
        <h2 class="content-title">Atlas: The Ultimate Guide to the World</h2>
        <p class="content-desc">Atlas is a website that lists every country with their flags and facts. You can explore
          the
          world map, search by<br>
          name or region, and filter by criteria. Learn about the world and its diversity with Atlas!</p>
      </li>
      <li>
        <button class="btn">filter</button>
      </li>
    </ul>



    <hr>
    <section>
      <ul class="cards">
        <li class="card">
          <!-- <li v-for="item in List" :key="item.id"> -->
          <img class="flag" src="\atlas.assets\de.png">
          <!-- {{ item.id }}-{{ item.title }} -->
          <div>
            <h3 class="country-name">Germany</h3>
            <p class="card-content">Federal Republic of Germany is an independent country in Western Europe with an
              estimated population of over
              83 million people.</p>
            <input type="chekbox">
          </div>
          <div>
            <button class="btn-2">Learn more</button>
          </div>
        </li>
      </ul>
    </section>
  </div>
</template>
<script setup>
// import JCard from 'vue';
// const List = [
//   {
//     id: nanoid(3),
//     flag: 'public\atlas.assets\de.png',
//     title: 'Germany',
//     desc: 'Federal Republic of Germany is an independent country in Western Europe with an estimated population of over 83 million people.'

//   },
//   {
//     id: nanoid(3),
//     flag: 'public\atlas.assets\de.png',
//     title: 'Paraguay',
//     desc: 'Republic of Paraguay is an independent country in South America with an estimated population of over 7.1 million people'
//   },
//   {
//     id: nanoid(3),
//     flag: '',
//     title: '',
//     desc: ''

//   },
//   {
//     id: nanoid(3),
//     flag: '',
//     title: '',
//     desc: ''

//   },
//   {
//     id: nanoid(3),
//     flag: '',
//     title: '',
//     desc: ''

//   },
//   {
//     id: nanoid(3),
//     flag: '',
//     title: '',
//     desc: ''

//   },
//   {
//     id: nanoid(3),
//     flag: '',
//     title: '',
//     desc: ''

//   },
//   {
//     id: nanoid(3),
//     flag: '',
//     title: '',
//     desc: ''

//   },
//   {
//     id: nanoid(3),
//     flag: '',
//     title: '',
//     desc: ''

//   },
//   {
//     id: nanoid(3),
//     flag: '',
//     title: '',
//     desc: ''

//   },
//   {
//     id: nanoid(3),
//     flag: '',
//     title: '',
//     desc: ''

//   },
//   {
//     id: nanoid(3),
//     flag: '',
//     title: '',
//     desc: ''

//   },

// ]

</script>
<style scoped>
.container {
  width: 1536px;
  height: 1620px;
  background-color: rgba(167, 179, 199, 1);
  padding-top: 20px;

}

.content {
  width: 1320px;
  height: auto;
  margin-top: 80px;
  margin-left: 108px;
  margin-right: 108px;
  display: flex;
  padding-bottom: 20px;

}

.content-1 {
  display: inline-block;

}

.content-title {
  font-family: Inter;
  font-size: 30px;
  font-weight: 600;
  line-height: 36px;
  letter-spacing: -0.04em;
  text-align: left;

}

.content-desc {
  font-family: Inter;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  letter-spacing: 0em;
  text-align: left;

}

.btn {
  width: 177px;
  height: 44px;
  padding: 4px;
  border-radius: 30px;
  border: 1px;
  gap: 4px;
  display: inline-block;
  margin-top: 10px;
  margin-left: 332px;
}

.card {
  /* width: 307.5px;
  height: 412px; */
  padding: 20px;
  border-radius: 10px;
  border: 1px;
  gap: 10px;
  background-color: rgba(255, 255, 255, 0.6);
  border: 1px solid rgba(255, 255, 255, 0.5)
}

.flag {
  width: 267.5px;
  height: 150px;
  border: 1px;
}

.country-name {
  font-family: Inter;
  font-size: 16px;
  font-weight: 700;
  line-height: 24px;
  letter-spacing: 0em;
  text-align: left;


}

.card-content {
  font-family: Inter;
  font-size: 14px;
  font-weight: 400;
  line-height: 20px;
  letter-spacing: 0em;
  text-align: left;
}

.btn-2 {
  width: 136px;
  height: 36px;
  padding: 8px, 16px, 8px, 16px;
  border-radius: 8px;
  border: 1px;
  gap: 8px;
}
</style>
