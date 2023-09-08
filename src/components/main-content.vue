<template>
    <div id="main-contant">
        <div id="cars-details">
            <div class="container">
                <div class="col-10 main-box">
                    <BreadCrumb />

                    <div class="row">
                        <div class="col-3">
                            <div id="srch-box">
                                <div id="title">
                                    <h6>Show Results By:</h6>
                                </div>
                                <div class="show-result-by">
                                   
                                    <SideBar />
                                </div>

                            </div>

                        </div>


                        <div class="col-9 ">
                            <CarsList />
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div id="contant-wrapper">
            <div class="container py-3">
                <div class="col-10 main-box">

                    <UsedCar />
                   
                </div>
            </div>
            <div id="Browse-cars">
                <div class="container pb-4">
                <div class="col-10 main-box">

                    
                    <BrowseMoreCar/>
                </div>
            </div>
            </div>
            <div class="container">
                <div class="col-10 pt-1 main-box">

                    <AppInstall/>
                   
                </div>
            </div>
            <div id="footer">
                <div class="container">
                <div class="col-10 main-box">

                    
                    <NavFooter/>
                </div>
            </div>
            </div>
            

        </div>
        <div id="sell-my-car">
            <div id="sell-car-wrapper">
                <i class="fa-solid fa-car"></i>
                Sell My Car
            </div>
        </div>

    </div>
</template>

<script>
import BreadCrumb from './breadCrumb.vue';

import SideBar from './sideBar.vue';
import CarsList from './CarsList.vue';
import UsedCar from './usedCar.vue';
import BrowseMoreCar from './Browse-more-car.vue';
import AppInstall from './app-install.vue';
import NavFooter from './nav-footer.vue';
export default {
    components: { BreadCrumb, SideBar, CarsList, UsedCar, BrowseMoreCar, AppInstall, NavFooter }
}
</script>

<style>
#footer {
    background: #23292f;
    border-top: 2px solid #181c20;
    color: #fff;
   
    font-size: 12px;
    line-height: 20px;
}

#Browse-cars{
    background-color: #f2f3f3;

}
#cars-details {
    background-color: #f2f3f3;
}

#main-contant .main-box {
    margin: 0px auto !important;
    padding-top: 35px;
    

}

/* Search box  */

#srch-box {
    background-color: #fcfcfc;
}

#srch-box #title h6 {
    background-color: #518ecb;
    color: #fff;
    padding: 9px 20px;
    text-transform: uppercase;
    font-size: 11px;
    line-height: 22px;
    margin: 0%;

}



.drop-down {
   
    font-size: 11px;
    border-top: 1px solid #EAEDEF;
    border-bottom: 1px solid #EAEDEF;
    line-height: 22px;
    text-transform: uppercase;
    font-weight: bold;
    padding: 9px 20px;
}

.drop-down i {
    float: right;
    line-height: 22px;
    font-size: 12px;

}
#sell-my-car #sell-car-wrapper{
    background-color: #b73439;
    color: #fff;
    padding: 13px 48px;
    border-radius: 30px;
}
#sell-my-car{
    position: fixed;
    bottom: 5%;
    right: 2%;
}
</style>