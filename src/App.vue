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

        <select class="btn">
          <option value="1">filter region</option>
          <option value="2">africa</option>
          <option value="3">american</option>
        </select>
      </li>
    </ul>
    <section>
      <JCard>
        <JFlag v-for="item in List" :key="item.id">
          <img class="flag" :src="item.flag">
          <template #title>{{ item.title }}</template>
          <template #desc>{{ item.desc }} </template>
          <!-- <ul class="cards"> -->
          <!-- <li class="card"> -->
          <!-- <li class="card" v-for="item in List" :key="item.id"> -->
          <!-- <img class="flag" src="/atlas.assets/de.png"> -->

          <!-- <h3 class="country-name">Germany</h3>
          <input name="check" id="check" type="checkbox">

          <p class="card-content">Federal Republic of Germany is an independent country in Western Europe with an
            estimated population of over
            83 million people.</p>
          <div>
            <button class="btn-2">
              <span class="btn-cont"> Learn more</span>
              <img class="icon" src="\atlas.assets\Icon (1).png">
            </button>
          </div> -->
          <!-- {{ item.title }}-{{ item.id }}-{{ item.desc }} -->
          <!-- </li> -->
        </JFlag>
      </JCard>
      <!-- </ul> -->
    </section>
  </div>
</template>
<script setup>
import { nanoid } from 'nanoid';
import JCard from '@/components/JCard.vue';
import JFlag from '@/components/JFlag.vue'
const List = [
  {
    id: nanoid(3),
    flag: 'public/atlas.assets/de.png',
    title: 'Germany',
    desc: 'Federal Republic of Germany is an independent country in Western Europe with an estimated population of over 83 million people.'

  },
  {
    id: nanoid(3),
    flag: 'public/atlas.assets/bf.png',
    title: 'IRAN',
    desc: ' is an independent country in Western Africa with an estimated population of over 20 million people.'

  },
  {
    id: nanoid(3),
    flag: 'public/atlas.assets/pn.png',
    title: 'Pitcairn Islands',
    desc: 'Pitcairn Islands is a dependent territory in Polynesia with an estimated population of over 56 people.'

  },
  {
    id: nanoid(3),
    flag: 'public/atlas.assets/de.png',
    title: 'Paraguay',
    desc: 'Republic of Paraguay is an independent country in South America with an estimated population of over 7.1 million people'
  },
  {
    id: nanoid(3),
    flag: 'public/atlas.assets/hk.png',
    title: 'Hong Kong',
    desc: 'Hong Kong Special Administrative Region of the Peoples Republic of China is a dependent territory in Eastern Asia  an estimated population of over 7.5 million people.'

  },

  {
    id: nanoid(3),
    flag: 'public/atlas.assets/bg.png',
    title: 'Bulgaria',
    desc: 'Republic of Bulgaria is an independent country in Southeast Europe with an estimated population of over 6.9 million people.'

  },
  {
    id: nanoid(3),
    flag: 'public/atlas.assets/bf.png',
    title: 'Antigua and Barbuda',
    desc: 'Antigua and Barbuda is an independent country in Caribbean with an estimated population of over 97 thousand people.'

  },
  {
    id: nanoid(3),
    flag: 'public/atlas.assets/ae.png',
    title: 'United Arab Emirates',
    desc: 'United Arab Emirates is an independent country in Western Asia with an estimated population of over 9.8 million people.'

  },
  {
    id: nanoid(3),
    flag: 'public/atlas.assets/dj.png',
    title: 'Djibouti',
    desc: 'Republic of Djibouti is an independent country in Eastern Africa with an estimated population of over 9.8 thousand people.'

  },
  {
    id: nanoid(3),
    flag: 'public/atlas.assets/in.png',
    title: 'India',
    desc: 'Republic of India is an independent country in Southern Asia with an estimated population of over 1.3 billion people.'

  },

  {
    id: nanoid(3),
    flag: 'public/atlas.assets/km.png',
    title: 'Comoros',
    desc: 'Union of the Comoros is an independent country in Eastern Africa with an estimated population of over 8.6 thousand people.'

  },
  {
    id: nanoid(3),
    flag: 'public/atlas.assets/la.png',
    title: 'Laos',
    desc: 'Lao Peoples Democratic Republic is an independent country in South - Eastern Asia with an estimated population of over 7.2 million people.'

  },

]

</script>
<style scoped>
.container {
  width: 1536px;
  height: 1620px;
  background-color: rgba(167, 179, 199, 1);
  padding-top: 20px;
  margin: auto;

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
  text-align: left;

}


/* .cards {
  display: inline-block;
  padding-left: 78px;
} */

.card {
  width: 307.5px;
  height: 412px;
  border-radius: 10px;
  border: 1px;
  gap: 10px;
  background-color: rgba(255, 255, 255, 0.6);
  border: 1px solid rgba(255, 255, 255, 0.5);
  display: inline-block;
  margin-left: 30px;
  margin-bottom: 30px;
  padding: 20px;
}

.flag {
  width: 267.5px;
  height: 150px;
  border: 1px solid rgba(255, 255, 255, 0.5);
  margin-bottom: 26px;
}

.title {
  font-family: Inter;
  font-size: 16px;
  font-weight: 700;
  line-height: 24px;
  letter-spacing: 0em;
  text-align: left;


}

/* .desc {
  font-family: Inter;
  font-size: 14px;
  font-weight: 400;
  line-height: 20px;
  letter-spacing: 0em;
  text-align: left;
  margin-bottom: 20px;
} */

/* .btn-2 {
  width: 136px;
  height: 36px;
  padding: 8px 16px 8px 16px;
  border-radius: 8px;
  border: 1px;
  gap: 8px;
  font-family: Inter;
  font-size: 14px;
  font-weight: 500;
  line-height: 20px;
  letter-spacing: 0em;
  text-align: left;
  color: rgba(0, 0, 0, 1);
  margin-top: 20px;



} */


.description {
  width: 267.5px;
  height: 166px;
  padding: 10px, 0px, 10px, 0px;
  gap: 10px;
}

/* .icon {
  width: 20px;
  height: 20px;
  margin-bottom: -5px;
  margin-right: -8px;
}

.btn-cont {
  font-family: Inter;
  font-size: 14px;
  font-weight: 500;
  line-height: 20px;
  letter-spacing: 0em;
  text-align: left;
  margin-top: 8px;
  margin-left: 16px;
  margin-bottom: 8px;
  margin-right: 8px;


} */

/* input {
  width: 36px;
  height: 36px;
  padding: 8px;
  border-radius: 36px;
  border: 1px;
  margin-left: 230px;
 

} */
</style>
