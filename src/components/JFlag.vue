<template>
    <li class="card">
        <slot class="flag">
        </slot>
        <!-- <h3 class="country">Germany</h3> -->
        <h3>
            <slot name="title" />
        </h3>
        <input name="check" id="check" type="checkbox">

        <!-- <p class="card-content"></p> -->
        <p>
            <slot name="desc" />
        </p>

        <div>
            <button class="btn-2">
                <span class="btn-cont"> Learn more</span>
                <img class="icon" src="\atlas.assets\Icon (1).png">
            </button>
        </div>



    </li>
</template>
<style scoped>
/* .card {
    width: 307.5px;
    height: 412px;
    padding: 20px;
    border-radius: 10px;
    border: 1px;
    gap: 10px;
    background-color: rgba(255, 255, 255, 0.6);
    border: 1px solid rgba(255, 255, 255, 0.5);
    display: inline-block;
    margin-left: 30px;
    margin-bottom: 30px;

} */
.desc {
    font-family: Inter;
    font-size: 14px;
    font-weight: 400;
    line-height: 20px;
    letter-spacing: 0em;
    text-align: left;
    /* margin-bottom: 200px; */
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

.desc {
    font-family: Inter;
    font-size: 14px;
    font-weight: 400;
    line-height: 20px;
    letter-spacing: 0em;
    text-align: left;
    margin-bottom: 20px;
}

.btn-2 {
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


}

.icon {
    width: 20px;
    height: 20px;
    margin-bottom: -5px;
    margin-right: -8px;
}

.btn-cont {
    margin-top: 8px;
    margin-left: 16px;
    margin-bottom: 8px;
    margin-right: 8px;
    font-family: Inter;
    font-size: 14px;
    font-weight: 500;
    line-height: 20px;
    letter-spacing: 0em;
    text-align: left;


}

input {
    width: 36px;
    height: 36px;
    padding: 8px;
    border-radius: 36px;
    border: 1px;
    margin-left: 230px;
    margin-top: -26px;

}
</style>