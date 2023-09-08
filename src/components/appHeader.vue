<template>
  <div id="header">
    <div id="login-header">
      <div class="container">
        <div class="row mt-1">
          <div class="col ">
            <div id="mobile-app" class="d-flex">
              <i class="fa-solid fa-mobile-screen-button text-danger"></i>
              <p class="m-0">
                Download App via SMS
              </p>
            </div>
          </div>

          <div class="col ">
            <ul id="login-menu">
              <li class="text-danger pe-1">
                <span> اردو </span>
              </li>
              <li class="login">
                <span> Sign Up</span>
              </li>
              <li class="login">
                <span> Sign In</span>
              </li>

            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <div id="main-header">
        <div class="row align-items-center">
          <div class="col-2 ">
            <img alt="PakWheels.com"
              src="https://wsa3.pakwheels.com/assets/new-pw-logo-f3b51e30f3761934b0a70973db08c32f.svg"
              title="PakWheels.com">
          </div>
          <div class="col-10  text-end">
            <ul id="main-menu">
              <li class="active">
                <a href="">Used cars
                  <i class="fa-solid fa-caret-down"></i>
                </a>
                <div class="dropdown-menu">
                  <ul class="dropdown-menu-wrapper">

                    <li>
                      <a href="/used-cars/search/-/" title="Used Cars Search">
                        <i class="fa fa-search"></i>
                        <strong>Find Used Cars for Sale</strong>
                        <p>Search from over 110k options</p>
                      </a>
                    </li>

                    <li>
                      <a href="/used-cars/search/-/featured_1/?nf=true">
                        <i class="fa fa-star"></i>
                        <strong>Featured Used Cars</strong>
                        <p>View featured cars by PakWheels</p>
                      </a>
                    </li>

                    <li>
                      <a href="/used-cars/sell" class="sign-in-comp">
                        <i class="fa fa-tag"></i>
                        <strong>Sell Your Car</strong>
                        <p>Post a free ad and sell your car quickly</p>
                      </a>
                    </li>

                    <li>
                      <a href="/used-cars/dealers/">
                        <i class="fa fa-book"></i>
                        <strong>Used Car Dealers</strong>
                        <p>Find used car dealers near your</p>
                      </a>
                    </li>

                    <li>
                      <a href="/used-cars/price-calculator/">
                        <i class="fa fa-bullseye"></i>
                        <strong>Price Calculator</strong>
                        <p>Calculate the market price of cars</p>
                      </a>
                    </li>

                  </ul>
                </div>

              </li>
              <li>
                <a href="#">New cars
                  <i class="fa-solid fa-caret-down"></i>

                </a>
                <div class="dropdown-menu">
                  <ul class="dropdown-menu-wrapper">

                    <li>
                      <a href="/new-cars/">
                        <i class="fa fa-search"></i>

                        <strong>Find New Cars</strong>
                        <p>See new cars in Pakistan</p>

                      </a>
                    </li>

                    <li>
                      <a href="/new-cars/compare/">
                        <i class="fa fa-columns"></i>
                        <strong>Car Comparisons</strong>
                        <p>Compare cars and find their differences</p>
                      </a>
                    </li>

                    <li>
                      <a href="/new-cars/reviews/">
                        <i class="fa fa-comments"></i>
                        <strong>Reviews</strong>
                        <p>Read reviews of all cars in Pakistan </p>
                      </a>
                    </li>

                    <li>
                      <a href="/new-cars/pricelist/">
                        <i class="fa fa-tags"></i>
                        <strong>Prices</strong>
                        <p>See prices of new cars</p>
                      </a>
                    </li>

                    <li>
                      <a href="/new-cars/on-road-price">
                        <i class="fa fa-road"></i>
                        <strong>On Road Price</strong>
                        <p>Calculate the total cost of new car</p>
                      </a>
                    </li>

                    <li>
                      <a href="/new-cars/dealers/">
                        <i class="fa fa-book"></i>
                        <strong>New Car Dealers</strong>
                        <p>Find new car dealers</p>
                      </a>
                    </li>

                  </ul>
                </div>

              </li>
              <li>
                <a href="#">Bikes
                  <i class="fa-solid fa-caret-down"></i>

                </a>
                <div class="dropdown-menu">
                  <ul class="dropdown-menu-wrapper">
                    <ul class="list-unstyled">

                      <li>
                        <a href="/used-bikes/" title="Motorcycles for sale in Pakistan">
                          <i class="fa fa-search"></i>
                          <strong>Find Used Bikes</strong>
                          <p>Find your dream bike</p>
                        </a>
                      </li>

                      <li>
                        <a href="/used-bikes/search/-/" title="Used Bikes Listings" rel="nofollow">
                          <i class="fa-solid fa-motorcycle"></i>
                          <strong>Used Bikes Listings</strong>
                          <p>Search from over 5000+ options</p>

                        </a>
                      </li>

                      <li>
                        <a href="/used-bikes/search/-/featured_1/">
                          <i class="fa fa-star"></i>
                          <strong>Featured Used Bikes</strong>
                          <p>Browse our featured bikes</p>

                        </a>
                      </li>

                      <li>
                        <a href="/used-bikes/sell">
                          <i class="fa fa-tag"></i>
                          <strong>Sell Your Bike</strong>
                          <p>Post a free ad and sell your bike quickly</p>
                        </a>
                      </li>

                    </ul>
                  </ul>
                </div>
              </li>
              <li>
                <a href="#">Auto Store
                  <i class="fa-solid fa-caret-down"></i>

                </a>
                <div class="dropdown-menu">
                  <ul class="dropdown-menu-wrapper">
                    <li><a class="dropdown-item" href="#">Action</a></li>
                    <li><a class="dropdown-item" href="#">Another action</a></li>
                    <li><a class="dropdown-item" href="#">Something else here</a></li>

                    <li><a class="dropdown-item" href="#">Separated link</a></li>
                  </ul>
                </div>
              </li>
              <li><a href="#">Video</a></li>
              <li><a href="#">Forums</a></li>
              <li><a href="#">Blog</a></li>
              <li>
                <a href="#">More
                  <i class="fa-solid fa-caret-down"></i>

                </a>
                <div class="dropdown-menu">
                  <ul class="dropdown-menu-wrapper">
                    <li><a class="dropdown-item" href="#">Action</a></li>
                    <li><a class="dropdown-item" href="#">Another action</a></li>
                    <li><a class="dropdown-item" href="#">Something else here</a></li>

                    <li><a class="dropdown-item" href="#">Separated link</a></li>

                  </ul>
                </div>
              </li>
              <li class=" post-an-ads">

                <a href="">

                  Post an Ad
                  <i class="fa-solid fa-caret-down"></i>
                </a>

                <div class="dropdown-menu">
                  <ul class="dropdown-menu-wrapper post-an-ads">
                    <li><a class="dropdown-item" href="#">Action</a></li>
                    <li><a class="dropdown-item" href="#">Another action</a></li>
                    <li><a class="dropdown-item" href="#">Something else here</a></li>
                    <li><a class="dropdown-item" href="#">Separated link</a></li>
                  </ul>
                </div>

              </li>
            </ul>
          </div>

        </div>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped>
#header {
  background-color: #fff;
  position: sticky;
  top: -33px;
  z-index: 999;
}

#main-header ul#main-menu>li:hover .dropdown-menu {
  max-height: 600px;
  border-bottom: 4px solid #b73439;


}

#main-header ul#main-menu .dropdown-menu-wrapper {
  padding: 30px 0px;
}

#main-header ul#main-menu>li>a i {
  font-size: 12px;
  max-width: 6px;
  display: inline-block;
  margin: 0;
  vertical-align: 3px;
}

#main-header .dropdown-menu {

  font-weight: normal;
  z-index: 99;
  margin: 0;
  border: none;
  box-shadow: 0 5px 5px rgb(0 0 0 / 30%);
  top: 45px;
  left: 0px;
  padding: 0;
  display: block;
  max-height: 0;
  transition: max-height .5s;
  overflow: hidden;
  width: max-content;

}

#main-header ul#main-menu .active>a {
  border-bottom: 5px solid #b73439;
}

.dropdown-menu i {
  float: left;
}

.dropdown-menu li a p {
  color: #7b8397;
  font-size: 12px;
  margin-bottom: 0;
  margin-top: -2px;
  line-height: 20px;
}

.dropdown-menu li a {
  display: block;
  padding-top: 5px;
  padding-right: 20px;
  padding-bottom: 15px;
  padding-left: 50px;
  color: #434343;
  text-decoration: none;
}


.dropdown-menu li a:hover {
  color: #518ecb !important;
}

.dropdown-menu li a strong {
  font-weight: 300;
  font-size: 16px;
  display: block;
  padding-bottom: 2px;
}

.dropdown-menu li a i {
  float: left;
  margin-left: -25px;
  margin-top: 4px;
  font-size: 13px;
}

#main-header li.post-an-ads>a {
  background-color: #b73439 !important;
  color: #fff !important;
  line-height: 40px;
  height: 40px;
  border-radius: 4px;
  margin-top: 5px;
  font-weight: 700;
  font-size: 15px;
}

#main-header li.post-an-ads {
  margin-left: 20px;
  margin-bottom: 15px;
}
</style>
