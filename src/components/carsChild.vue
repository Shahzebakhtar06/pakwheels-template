<template>
    <div class="cars">
        <div class="cars-item">
            <div class="row">
                <div class="col-3 pe-2">
                    <div class="feature-info">
                        <div class="feature-ribbon">
                            FEATURED
                            <i class="fa fa-exclamation-circle"></i>
                        </div>
                    </div>
                    <div class="img">
                        <img class="pic"
                            :src="imgPath">
                    </div>
                </div>
                <div class="col-9">
                    <div class="title">
                        <div class="row">
                            <div class="col-9 cars-name">
                                <h6>{{header}}</h6>
                            </div>
                            <div class="col-3 p-0">
                                <div class="price">
                                  PKR {{price}} lacs
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="cars-city mb-2">
                        {{carCity}}
                    </div>
                    <div class="cars-details">
                        <ul class="carDetails">
                            <li>{{carDetails.year}}</li>
                            <li>{{carDetails.km}} km</li>
                            <li>{{carDetails.comp}}</li>
                            <li>{{carDetails.cc}} cc</li>
                            <li>{{carDetails.type}}</li>
                        </ul>
                    </div>
                    <div class="clint-details">
                        <div class="row">
                            <div class="col">
                                <div class="pull-left dated">{{updateTime}}</div>

                                <div>
                                </div>

                            </div>
                            <div class="col text-end phone">
                                <div class="heart-icon">
                                    <i class="fa-regular fa-heart"></i>
                                </div>

                                <button>
                                    <i class="fa fa-phone"></i>Show Phone No.
                                </button>
                            </div>

                        </div>
                    </div>
                </div>
            </div>
        </div>

    </div>
</template>

<script>
export default {
    data() {
        return {
            // carDetailss: "",
        }
    },
    // props: {
    //     header: String,
    //     price: String,
    //     carCity: String,
    //     updateTime: String,
    //     carDetails: Object
    // },
    props: ["header", "price", "carCity", "updateTime", "carDetails","imgPath"],

}
</script>

<style>

</style>
