
<template>
    <div class="sort">
        <div class="organize-results row">
            <div class="col-md-8">
                <span class="">
                    <span class="sort-by-text">Sort By: </span>
                    <select id="sortby" name="sortby">
                        <option value="bumped_at-desc">Updated Date: Recent First</option>
                        <option value="bumped_at-asc">Updated Date: Oldest First</option>
                        <option value="price-asc">Price: Low to High</option>
                        <option value="price-desc">Price: High to Low</option>
                        <option value="model_year-desc">Model Year: Latest First</option>
                        <option value="model_year-asc">Model Year: Oldest First</option>
                        <option value="mileage-asc">Mileage: Low to High</option>
                        <option value="mileage-desc">Mileage: High to Low</option>
                    </select>
                </span>
            </div>

            <div class="col-md-4 mt-1 text-end sort-view">
                <div class="btn-group" data-toggle="buttons-radio">
                    <button type="button" id="list" class="btn btn-sm active ">
                        <span class="generic-dark-grey "><i class="fa fa-th-list"></i> LIST</span>
                    </button>
                    <button type="button" id="grid" class="btn btn-sm ">
                        <span class="generic-dark-grey"><i class="fa fa-th-large"></i> GRID</span>
                    </button>
                </div>
            </div>
        </div>
    </div>

    <div class="cars">
        <CarsChild v-for="item in getCarsData" :key="item.id" :header="item.header" :price="item.price"
            :carCity="item.carCity" :updateTime="item.updateTime" :carDetails="item.carDetails" :imgPath="item.imgPath" />

        <div id="pagination">
            <div data-pjax-enable="">
                <ul class="pagination search-pagi">

                    <li class="page active">
                        <a href="/used-cars/search/-/">1</a>
                    </li>

                    <li class="page">
                        <a href="/used-cars/search/-/?page=2" rel="next">2</a>
                    </li>

                    <li class="page">
                        <a href="/used-cars/search/-/?page=3">3</a>
                    </li>

                    <li class="page">
                        <a href="/used-cars/search/-/?page=4">4</a>
                    </li>

                    <li class="page">
                        <a href="/used-cars/search/-/?page=5">5</a>
                    </li>

                    <li class="page gap disabled"><a href="#" onclick="return false;">…</a></li>
                    <li class="next_page">
                        <a href="/used-cars/search/-/?page=2" rel="next">Next ›</a>
                    </li>

                    <li class="last next">
                        <a href="/used-cars/search/-/?page=3561">Last »</a>
                    </li>
                
                </ul>

            </div>
        </div>
        <div id="sell-ads">
            <div class="sell-ad-widget clearfix text-center p20">

                <img src="https://wsa4.pakwheels.com/assets/sell-car-bf334aeb9cf3001080a3e887d51a3b32.png">

                <h3 class="title">Post an ad for <span class="text-danger">FREE</span></h3>
                <p class="mt10 mb5 fs16">Sell it faster to thousands of buyers</p>
                <div>
                    <img alt="Post an Ad Left"
                        src="https://wsa4.pakwheels.com/assets/sell-ad-point-left-fcc7bca4d40628d7945426ecf5a2ef00.png">
                    <a href="/used-cars/sell" class="btn btn-success sign-in-comp">Sell Your Car</a>
                    <img
                        src="https://wsa4.pakwheels.com/assets/sell-ad-point-right-630620add9bbdd27360acdfcf98d0608.png">
                </div>
            </div>
        </div>
        <div id="services-icon">
            <div class="services-icon-item">
                <i class="fa-brands fa-facebook-f"></i>
            </div>
            <div class="services-icon-item">
                <i class="fa-brands fa-twitter"></i>
            </div>
            <div class="services-icon-item">
                <i class="fa-solid fa-print"></i>
            </div>
            <div class="services-icon-item">
                <i class="fa fa-sms"></i>
            </div>
            <div class="services-icon-item">
                <i class="fa-solid fa-plus"></i>
            </div>

        </div>
    </div>

</template>

<script>
import CarsChild from './carsChild.vue';
import { mapGetters } from 'vuex'

export default {
    data() {
        return {
        }
        
    },

    components: { CarsChild },
    computed: {
    ...mapGetters([
      'getCarsData',
      'getData'
    ])
  },
    mounted (){
      
        
    },
    methods:{
 
    }
}
</script>

<style>
.sort {
    background-color: #fff;
    border: 1px solid #e6e6e6;
    padding: 10px 20px;
    font-size: 14px;
    line-height: 1.4287;
    color: #434343;
}

.sort-view {
    color: #434343;

}

.sort-view button {
    border: 1px solid #e6e6e6;
    font-size: 10px;
    padding: 2px 9px;

}

#sortby {
    height: 28px;
    padding: 2px;
    font-size: 12px !important;
    width: 200px;
    margin: 0;
    outline: none;
    border: 1px solid #e6e6e6;
    background-color: #fff;
    border-radius: 4px;
    color: #434343;
}

.sort .sort-view .active {
    box-shadow: 0px 4px 5px #e6e6e6 inset !important;
    outline: none;
    border: 1px solid #e6e6e6;

}

.sort .sort-view i {
    vertical-align: 2px;
}

.sort-by-text {
    float: left;
    margin-right: 10px;
    font-size: 12px;
    line-height: 20px;
    color: #7b8397;
}

.cars .btn-group button {
    outline: none;
    padding: 2px 8px 0;
    font-size: 11px;
    vertical-align: middle;
    border: 1px solid #e6e6e6;

}

.cars-item {
    background-color: #fff;
    font-size: 13px;
    padding: 11px;
    margin: 20px 0px;
    position: relative;
    border: 2px solid #e6e6e6;
}

.cars-item img {
    width: 100%;
}

div.cars-name h6 {
    color: #233d7b;
    font-weight: bold;
    line-height: 22px;
    font-size: 15px;
}

.title h6:hover {
    color: #518ecb;
}

.price {
    font-size: 18px;
    font-weight: 700;
    line-height: normal;
    color: #464e60;
    text-align: center;
}

.pull-left.dated {
    font-size: 11px;
    line-height: 27px;
}

.clint-details {
    margin-top: -6px;
}

.carDetails {
    display: flex;
    padding: 0%;
}

.carDetails li {
    list-style: none;

}

.carDetails li:after {
    content: "|";
    padding-top: 0px;
    padding-right: 7px;
    padding-bottom: 0px;
    padding-left: 10px;
    color: #cbd4d9;
    vertical-align: 1px;
}

.heart-icon i {
    border: 1px solid #EAEDEF;
    cursor: pointer;
    padding: 1px 12px;
    border-radius: 2px;
    margin-right: 5px;
    line-height: 22px;

}

.phone button {
    color: #fff;
    background-color: #3eb549;
    border-color: #37a241;
    outline: none;
    border: none;
    padding: 1px 12px;
    font-size: 11px;
}

.phone button i {

    margin-right: 8px !important;

}

.phone {
    display: flex;
    justify-content: end;
}

.feature-ribbon {
    position: absolute;
    z-index: 6;
    background-color: #b73439;
    color: #fff;
    line-height: 18px;
    font-size: 11px;
    font-weight: 400;
    left: 0;
    top: 0;
    padding: 5px;
}

#pagination ul.search-pagi li a {
    padding: 5px;
    color: #518ecb;
    text-decoration: none;
}

#pagination ul.search-pagi {
    box-shadow: none;
    display: block;
    background-color: #ffffff;
    border: 1px solid #EAEDEF;
    text-align: center;
    padding: 19px;
    font-size: 16px;
    clear: both;
    margin-top: 0;
    margin-bottom: 20px;
    display: flex;
    justify-content: center;
}

#sell-ads {
    padding: 45px 50px 58px;
}

#sell-ads p {
    margin-bottom: 3px;
}

#sell-ads .btn-success {
    color: #fff;
    background-color: #3eb549;
    border-color: #37a241;
    outline: none;
    border: none;
    vertical-align: -17px;
    margin: 0 20px;
    font-size: 18px;
    font-weight: 700;
    padding: 6px 25px;

}

#sell-ads .title {
    color: #233d7b;
    font-size: 1.4rem;
    font-weight: bold;
    margin-top: 10px;


}

.cars #services-icon {
    position: fixed;
    top: 20%;
    left: 0;

}

.cars #services-icon .services-icon-item {
    font-size: 21px;
    color: #fff;
    width: 3pc;
    padding: 8px 0;
    text-align: center;
}

.cars #services-icon .services-icon-item:first-child {
    background-color: rgb(59, 89, 152);
}

.cars #services-icon .services-icon-item:nth-child(2) {
    background-color: rgb(29, 161, 242);
}

.cars #services-icon .services-icon-item:nth-child(3) {
    background-color: rgb(115, 138, 141);
}

.cars #services-icon .services-icon-item:nth-child(4) {
    background-color: rgb(132, 132, 132);

}

.cars #services-icon .services-icon-item:nth-child(5) {

    background-color: rgb(255, 101, 80);
}
</style>
