
<template>
    <div id="check-boxes" class="p-0">

        <div id="key-srch" class="title">
            <div class="drop-down" data-bs-auto-close="false" data-bs-toggle="dropdown">
                Search by Keyword
                <i class="fa-solid fa-caret-down"></i>
            </div>
            <div class="dropdown-menu" aria-labelledby="dropdown">
                <div class="srch-bar">
                    <div class="srch-wrapper">
                        <input type="text" placeholder="e.g. Honda in Lahore">
                        <span class="go-btn">Go</span>
                    </div>
                </div>
            </div>
        </div>
        <div id="city">
            <div class="drop-down" data-bs-auto-close="false" data-bs-toggle="dropdown">
                city
                <i class="fa-solid fa-caret-down"></i>
            </div>
            <div class="drop-down-menu default-city">

                <ul class="dropdown-menu" aria-labelledby="city">
                    <li>
                        <input type="checkbox" value="lahore" v-model="filtered.City">
                        Lahore
                        <span>18460</span>
                    </li>
                    <li>
                        <input type="checkbox" value="karachi" v-model="filtered.City">
                        Karachi
                        <span>18174</span>
                    </li>
                    <li>
                        <input type="checkbox" value="islamabad" v-model="filtered.City">
                        Islamabad
                        <span>12949</span>
                    </li>
                    <li>
                        <input type="checkbox" value="rawalpindi" v-model="filtered.City">
                        Rawalpindi
                        <span>5992</span>
                    </li>
                    <li>
                        <input type="checkbox" value="peshawar" v-model="filtered.City">
                        Peshawar
                        <span>4266</span>
                    </li>
                    <li>
                        <a class="more-choice" data-bs-toggle="modal" data-bs-target="#lb_more_choices_cities" rel=""
                            aria-labelledby="exampleModalLabel" aria-hidden="true">more
                            choices...</a>
                    </li>

                </ul>

            </div>
            <div id="lb_more_choices_cities" class="modal more_choices_cities in" tabindex="-1">

                <div class="modal-dialog" id="more_choices_cities">
                    <div class="modal-content">
                        <div class="modal-header">
                            <button type="button" class="close" data-bs-dismiss="modal" aria-hidden="true">×</button>
                            <h4> Select City</h4>
                        </div>

                        <form method="get">
                            <div class="modal-body checkbox-list">
                                <ul id="city_list_popular" name="city_list"
                                    class="list-unstyled d-inline list-links clearfix">
                                    <li>
                                        <label class="checkbox">
                                            <input value="lahore" type="checkbox">
                                            <a href="/used-cars/lahore/24858 " data-dismiss="modal"
                                                style="color: #353944">
                                                Lahore <span class="badge badge-gray-light pull-right">18788</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="karachi" type="checkbox">
                                            <a href="/used-cars/karachi/24857 " data-dismiss="modal"
                                                style="color: #353944">
                                                Karachi <span class="badge badge-gray-light pull-right">18488</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="islamabad" type="checkbox">
                                            <a href="/used-cars/islamabad/24856 " data-dismiss="modal"
                                                style="color: #353944">
                                                Islamabad <span class="badge badge-gray-light pull-right">13076</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="rawalpindi" type="checkbox">
                                            <a href="/used-cars/rawalpindi/24831 " data-dismiss="modal"
                                                style="color: #353944">
                                                Rawalpindi <span class="badge badge-gray-light pull-right">5938</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="peshawar" type="checkbox">
                                            <a href="/used-cars/peshawar/24821 " data-dismiss="modal"
                                                style="color: #353944">
                                                Peshawar <span class="badge badge-gray-light pull-right">4362</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="quetta" type="checkbox">
                                            <a href="/used-cars/quetta/24826 " data-dismiss="modal"
                                                style="color: #353944">
                                                Quetta <span class="badge badge-gray-light pull-right">632</span>
                                            </a>
                                        </label>
                                    </li>
                                </ul>
                                <h4 style="margin: 10px 0 5px;">More Cities</h4>
                                <ul id="city_list" name="city_list" class="list-unstyled inline list-links clearfix">
                                    <li>
                                        <label class="checkbox">
                                            <input value="abbottabad" type="checkbox">
                                            <a href="/used-cars/abbottabad/727521 " data-dismiss="modal"
                                                style="color: #353944">
                                                Abbottabad <span class="badge badge-gray-light pull-right">804</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="ahmed-pur-east" type="checkbox">
                                            <a href="/used-cars/ahmed-pur-east/107673 " data-dismiss="modal"
                                                style="color: #353944">
                                                Ahmed Pur East <span class="badge badge-gray-light pull-right">40</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="arifwala" type="checkbox">
                                            <a href="/used-cars/arifwala/24728 " data-dismiss="modal"
                                                style="color: #353944">
                                                Arifwala <span class="badge badge-gray-light pull-right">75</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="attock" type="checkbox">
                                            <a href="/used-cars/attock/24729 " data-dismiss="modal"
                                                style="color: #353944">
                                                Attock <span class="badge badge-gray-light pull-right">397</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="bahawalnagar" type="checkbox">
                                            <a href="/used-cars/bahawalnagar/24731 " data-dismiss="modal"
                                                style="color: #353944">
                                                Bahawalnagar <span class="badge badge-gray-light pull-right">124</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="bahawalpur" type="checkbox">
                                            <a href="/used-cars/bahawalpur/24732 " data-dismiss="modal"
                                                style="color: #353944">
                                                Bahawalpur <span class="badge badge-gray-light pull-right">803</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="bannu" type="checkbox">
                                            <a href="/used-cars/bannu/24734 " data-dismiss="modal"
                                                style="color: #353944">
                                                Bannu <span class="badge badge-gray-light pull-right">107</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="bhakkar" type="checkbox">
                                            <a href="/used-cars/bhakkar/24736 " data-dismiss="modal"
                                                style="color: #353944">
                                                Bhakkar <span class="badge badge-gray-light pull-right">127</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="bhalwal" type="checkbox">
                                            <a href="/used-cars/bhalwal/25872 " data-dismiss="modal"
                                                style="color: #353944">
                                                Bhalwal <span class="badge badge-gray-light pull-right">60</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="burewala" type="checkbox">
                                            <a href="/used-cars/burewala/24738 " data-dismiss="modal"
                                                style="color: #353944">
                                                Burewala <span class="badge badge-gray-light pull-right">170</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="chakwal" type="checkbox">
                                            <a href="/used-cars/chakwal/24739 " data-dismiss="modal"
                                                style="color: #353944">
                                                Chakwal <span class="badge badge-gray-light pull-right">361</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="charsadda" type="checkbox">
                                            <a href="/used-cars/charsadda/68113 " data-dismiss="modal"
                                                style="color: #353944">
                                                Charsadda <span class="badge badge-gray-light pull-right">209</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="chichawatni" type="checkbox">
                                            <a href="/used-cars/chichawatni/71432 " data-dismiss="modal"
                                                style="color: #353944">
                                                Chichawatni <span class="badge badge-gray-light pull-right">102</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="chiniot" type="checkbox">
                                            <a href="/used-cars/chiniot/24743 " data-dismiss="modal"
                                                style="color: #353944">
                                                Chiniot <span class="badge badge-gray-light pull-right">103</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="chishtian" type="checkbox">
                                            <a href="/used-cars/chishtian/24744 " data-dismiss="modal"
                                                style="color: #353944">
                                                Chishtian <span class="badge badge-gray-light pull-right">61</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="d-g-khan" type="checkbox">
                                            <a href="/used-cars/d-g-khan/68114 " data-dismiss="modal"
                                                style="color: #353944">
                                                D.G.Khan <span class="badge badge-gray-light pull-right">340</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="daska" type="checkbox">
                                            <a href="/used-cars/daska/24746 " data-dismiss="modal"
                                                style="color: #353944">
                                                Daska <span class="badge badge-gray-light pull-right">92</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="depal-pur" type="checkbox">
                                            <a href="/used-cars/depal-pur/24747 " data-dismiss="modal"
                                                style="color: #353944">
                                                Depal pur <span class="badge badge-gray-light pull-right">51</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="dera-ismail-khan" type="checkbox">
                                            <a href="/used-cars/dera-ismail-khan/24749 " data-dismiss="modal"
                                                style="color: #353944">
                                                Dera ismail khan <span
                                                    class="badge badge-gray-light pull-right">157</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="dina" type="checkbox">
                                            <a href="/used-cars/dina/24751 " data-dismiss="modal"
                                                style="color: #353944">
                                                Dina <span class="badge badge-gray-light pull-right">37</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="dinga" type="checkbox">
                                            <a href="/used-cars/dinga/24752 " data-dismiss="modal"
                                                style="color: #353944">
                                                Dinga <span class="badge badge-gray-light pull-right">37</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="faisalabad" type="checkbox">
                                            <a href="/used-cars/faisalabad/24753 " data-dismiss="modal"
                                                style="color: #353944">
                                                Faisalabad <span class="badge badge-gray-light pull-right">3547</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="fateh-jang" type="checkbox">
                                            <a href="/used-cars/fateh-jang/71026 " data-dismiss="modal"
                                                style="color: #353944">
                                                Fateh Jang <span class="badge badge-gray-light pull-right">85</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="gojra" type="checkbox">
                                            <a href="/used-cars/gojra/24760 " data-dismiss="modal"
                                                style="color: #353944">
                                                Gojra <span class="badge badge-gray-light pull-right">105</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="gujar-khan" type="checkbox">
                                            <a href="/used-cars/gujar-khan/69505 " data-dismiss="modal"
                                                style="color: #353944">
                                                Gujar Khan <span class="badge badge-gray-light pull-right">118</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="gujranwala" type="checkbox">
                                            <a href="/used-cars/gujranwala/24763 " data-dismiss="modal"
                                                style="color: #353944">
                                                Gujranwala <span class="badge badge-gray-light pull-right">2177</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="gujrat" type="checkbox">
                                            <a href="/used-cars/gujrat/24764 " data-dismiss="modal"
                                                style="color: #353944">
                                                Gujrat <span class="badge badge-gray-light pull-right">766</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="hafizabad" type="checkbox">
                                            <a href="/used-cars/hafizabad/24765 " data-dismiss="modal"
                                                style="color: #353944">
                                                Hafizabad <span class="badge badge-gray-light pull-right">125</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="haripur--2" type="checkbox">
                                            <a href="/used-cars/haripur--2/739930 " data-dismiss="modal"
                                                style="color: #353944">
                                                Haripur <span class="badge badge-gray-light pull-right">237</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="haroonabad" type="checkbox">
                                            <a href="/used-cars/haroonabad/45823 " data-dismiss="modal"
                                                style="color: #353944">
                                                Haroonabad <span class="badge badge-gray-light pull-right">47</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="hasilpur" type="checkbox">
                                            <a href="/used-cars/hasilpur/24767 " data-dismiss="modal"
                                                style="color: #353944">
                                                Hasilpur <span class="badge badge-gray-light pull-right">52</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="hassan-abdal" type="checkbox">
                                            <a href="/used-cars/hassan-abdal/24768 " data-dismiss="modal"
                                                style="color: #353944">
                                                Hassan abdal <span class="badge badge-gray-light pull-right">46</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="hyderabad" type="checkbox">
                                            <a href="/used-cars/hyderabad/24771 " data-dismiss="modal"
                                                style="color: #353944">
                                                Hyderabad <span class="badge badge-gray-light pull-right">971</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="jaranwala" type="checkbox">
                                            <a href="/used-cars/jaranwala/24774 " data-dismiss="modal"
                                                style="color: #353944">
                                                Jaranwala <span class="badge badge-gray-light pull-right">64</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="jauharabad" type="checkbox">
                                            <a href="/used-cars/jauharabad/24775 " data-dismiss="modal"
                                                style="color: #353944">
                                                Jauharabad <span class="badge badge-gray-light pull-right">47</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="jhang" type="checkbox">
                                            <a href="/used-cars/jhang/24778 " data-dismiss="modal"
                                                style="color: #353944">
                                                Jhang <span class="badge badge-gray-light pull-right">246</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="jhelum" type="checkbox">
                                            <a href="/used-cars/jhelum/24779 " data-dismiss="modal"
                                                style="color: #353944">
                                                Jhelum <span class="badge badge-gray-light pull-right">374</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="kamoke" type="checkbox">
                                            <a href="/used-cars/kamoke/107291 " data-dismiss="modal"
                                                style="color: #353944">
                                                Kamoke <span class="badge badge-gray-light pull-right">42</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="karak" type="checkbox">
                                            <a href="/used-cars/karak/24786 " data-dismiss="modal"
                                                style="color: #353944">
                                                Karak <span class="badge badge-gray-light pull-right">39</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="kashmir" type="checkbox">
                                            <a href="/used-cars/kashmir/24787 " data-dismiss="modal"
                                                style="color: #353944">
                                                Kashmir <span class="badge badge-gray-light pull-right">41</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="kasur" type="checkbox">
                                            <a href="/used-cars/kasur/24788 " data-dismiss="modal"
                                                style="color: #353944">
                                                Kasur <span class="badge badge-gray-light pull-right">114</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="khanewal" type="checkbox">
                                            <a href="/used-cars/khanewal/24790 " data-dismiss="modal"
                                                style="color: #353944">
                                                Khanewal <span class="badge badge-gray-light pull-right">101</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="khanpur--2" type="checkbox">
                                            <a href="/used-cars/khanpur--2/677247 " data-dismiss="modal"
                                                style="color: #353944">
                                                Khanpur <span class="badge badge-gray-light pull-right">79</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="kharian" type="checkbox">
                                            <a href="/used-cars/kharian/24791 " data-dismiss="modal"
                                                style="color: #353944">
                                                Kharian <span class="badge badge-gray-light pull-right">145</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="khushab" type="checkbox">
                                            <a href="/used-cars/khushab/24792 " data-dismiss="modal"
                                                style="color: #353944">
                                                Khushab <span class="badge badge-gray-light pull-right">117</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="kohat" type="checkbox">
                                            <a href="/used-cars/kohat/24793 " data-dismiss="modal"
                                                style="color: #353944">
                                                Kohat <span class="badge badge-gray-light pull-right">206</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="kot-addu" type="checkbox">
                                            <a href="/used-cars/kot-addu/24794 " data-dismiss="modal"
                                                style="color: #353944">
                                                Kot addu <span class="badge badge-gray-light pull-right">51</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="kotli-ak" type="checkbox">
                                            <a href="/used-cars/kotli-ak/750385 " data-dismiss="modal"
                                                style="color: #353944">
                                                Kotli Ak <span class="badge badge-gray-light pull-right">47</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="lala-musa" type="checkbox">
                                            <a href="/used-cars/lala-musa/24796 " data-dismiss="modal"
                                                style="color: #353944">
                                                Lala musa <span class="badge badge-gray-light pull-right">45</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="larkana" type="checkbox">
                                            <a href="/used-cars/larkana/24797 " data-dismiss="modal"
                                                style="color: #353944">
                                                Larkana <span class="badge badge-gray-light pull-right">39</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="layyah" type="checkbox">
                                            <a href="/used-cars/layyah/24798 " data-dismiss="modal"
                                                style="color: #353944">
                                                Layyah <span class="badge badge-gray-light pull-right">132</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="lodhran" type="checkbox">
                                            <a href="/used-cars/lodhran/50850 " data-dismiss="modal"
                                                style="color: #353944">
                                                Lodhran <span class="badge badge-gray-light pull-right">58</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="mandi-bahauddin" type="checkbox">
                                            <a href="/used-cars/mandi-bahauddin/24802 " data-dismiss="modal"
                                                style="color: #353944">
                                                Mandi bahauddin <span
                                                    class="badge badge-gray-light pull-right">324</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="mansehra" type="checkbox">
                                            <a href="/used-cars/mansehra/752719 " data-dismiss="modal"
                                                style="color: #353944">
                                                Mansehra <span class="badge badge-gray-light pull-right">311</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="mardan" type="checkbox">
                                            <a href="/used-cars/mardan/24805 " data-dismiss="modal"
                                                style="color: #353944">
                                                Mardan <span class="badge badge-gray-light pull-right">776</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="mian-channu" type="checkbox">
                                            <a href="/used-cars/mian-channu/72363 " data-dismiss="modal"
                                                style="color: #353944">
                                                Mian Channu <span class="badge badge-gray-light pull-right">78</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="mian-wali" type="checkbox">
                                            <a href="/used-cars/mian-wali/68117 " data-dismiss="modal"
                                                style="color: #353944">
                                                Mian Wali <span class="badge badge-gray-light pull-right">152</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="mirpur-a-k" type="checkbox">
                                            <a href="/used-cars/mirpur-a-k/68118 " data-dismiss="modal"
                                                style="color: #353944">
                                                Mirpur A.K. <span class="badge badge-gray-light pull-right">237</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="mirpur-khas" type="checkbox">
                                            <a href="/used-cars/mirpur-khas/24809 " data-dismiss="modal"
                                                style="color: #353944">
                                                Mirpur khas <span class="badge badge-gray-light pull-right">70</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="multan" type="checkbox">
                                            <a href="/used-cars/multan/24810 " data-dismiss="modal"
                                                style="color: #353944">
                                                Multan <span class="badge badge-gray-light pull-right">2729</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="muridke" type="checkbox">
                                            <a href="/used-cars/muridke/756807 " data-dismiss="modal"
                                                style="color: #353944">
                                                Muridke <span class="badge badge-gray-light pull-right">36</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="murree" type="checkbox">
                                            <a href="/used-cars/murree/24811 " data-dismiss="modal"
                                                style="color: #353944">
                                                Murree <span class="badge badge-gray-light pull-right">40</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="muzaffar-gargh" type="checkbox">
                                            <a href="/used-cars/muzaffar-gargh/68119 " data-dismiss="modal"
                                                style="color: #353944">
                                                Muzaffar Gargh <span
                                                    class="badge badge-gray-light pull-right">106</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="muzaffarabad" type="checkbox">
                                            <a href="/used-cars/muzaffarabad/24812 " data-dismiss="modal"
                                                style="color: #353944">
                                                Muzaffarabad <span class="badge badge-gray-light pull-right">99</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="nankana-sahib" type="checkbox">
                                            <a href="/used-cars/nankana-sahib/24814 " data-dismiss="modal"
                                                style="color: #353944">
                                                Nankana sahib <span class="badge badge-gray-light pull-right">66</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="narowal" type="checkbox">
                                            <a href="/used-cars/narowal/30890 " data-dismiss="modal"
                                                style="color: #353944">
                                                Narowal <span class="badge badge-gray-light pull-right">77</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="nawabshah" type="checkbox">
                                            <a href="/used-cars/nawabshah/69292 " data-dismiss="modal"
                                                style="color: #353944">
                                                Nawabshah <span class="badge badge-gray-light pull-right">55</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="nowshera" type="checkbox">
                                            <a href="/used-cars/nowshera/24816 " data-dismiss="modal"
                                                style="color: #353944">
                                                Nowshera <span class="badge badge-gray-light pull-right">233</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="nowshera-cantt" type="checkbox">
                                            <a href="/used-cars/nowshera-cantt/24817 " data-dismiss="modal"
                                                style="color: #353944">
                                                Nowshera cantt <span class="badge badge-gray-light pull-right">81</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="okara" type="checkbox">
                                            <a href="/used-cars/okara/24818 " data-dismiss="modal"
                                                style="color: #353944">
                                                Okara <span class="badge badge-gray-light pull-right">298</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="pak-pattan-sharif" type="checkbox">
                                            <a href="/used-cars/pak-pattan-sharif/24819 " data-dismiss="modal"
                                                style="color: #353944">
                                                Pak pattan sharif <span
                                                    class="badge badge-gray-light pull-right">77</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="pasrur" type="checkbox">
                                            <a href="/used-cars/pasrur/758414 " data-dismiss="modal"
                                                style="color: #353944">
                                                Pasrur <span class="badge badge-gray-light pull-right">42</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="pattoki" type="checkbox">
                                            <a href="/used-cars/pattoki/107448 " data-dismiss="modal"
                                                style="color: #353944">
                                                Pattoki <span class="badge badge-gray-light pull-right">52</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="pindi-bhattian" type="checkbox">
                                            <a href="/used-cars/pindi-bhattian/759255 " data-dismiss="modal"
                                                style="color: #353944">
                                                Pindi Bhattian <span class="badge badge-gray-light pull-right">36</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="pindi-gheb" type="checkbox">
                                            <a href="/used-cars/pindi-gheb/24824 " data-dismiss="modal"
                                                style="color: #353944">
                                                Pindi gheb <span class="badge badge-gray-light pull-right">35</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="pir-mahal" type="checkbox">
                                            <a href="/used-cars/pir-mahal/24825 " data-dismiss="modal"
                                                style="color: #353944">
                                                Pir mahal <span class="badge badge-gray-light pull-right">60</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="rahim-yar-khan" type="checkbox">
                                            <a href="/used-cars/rahim-yar-khan/68120 " data-dismiss="modal"
                                                style="color: #353944">
                                                Rahim Yar Khan <span
                                                    class="badge badge-gray-light pull-right">512</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="rawat" type="checkbox">
                                            <a href="/used-cars/rawat/47518 " data-dismiss="modal"
                                                style="color: #353944">
                                                Rawat <span class="badge badge-gray-light pull-right">51</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="sadiqabad" type="checkbox">
                                            <a href="/used-cars/sadiqabad/24833 " data-dismiss="modal"
                                                style="color: #353944">
                                                Sadiqabad <span class="badge badge-gray-light pull-right">132</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="sahiwal" type="checkbox">
                                            <a href="/used-cars/sahiwal/24834 " data-dismiss="modal"
                                                style="color: #353944">
                                                Sahiwal <span class="badge badge-gray-light pull-right">459</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="sargodha" type="checkbox">
                                            <a href="/used-cars/sargodha/24836 " data-dismiss="modal"
                                                style="color: #353944">
                                                Sargodha <span class="badge badge-gray-light pull-right">988</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="sheikhupura" type="checkbox">
                                            <a href="/used-cars/sheikhupura/24838 " data-dismiss="modal"
                                                style="color: #353944">
                                                Sheikhupura <span class="badge badge-gray-light pull-right">221</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="sheikhupura--2" type="checkbox">
                                            <a href="/used-cars/search/-/ct_sheikhupura--2/ " data-dismiss="modal"
                                                style="color: #353944" rel="nofollow">
                                                Sheikhupura <span class="badge badge-gray-light pull-right">75</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="shorkot" type="checkbox">
                                            <a href="/used-cars/shorkot/24840 " data-dismiss="modal"
                                                style="color: #353944">
                                                Shorkot <span class="badge badge-gray-light pull-right">34</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="sialkot" type="checkbox">
                                            <a href="/used-cars/sialkot/24841 " data-dismiss="modal"
                                                style="color: #353944">
                                                Sialkot <span class="badge badge-gray-light pull-right">1343</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="sukkur" type="checkbox">
                                            <a href="/used-cars/sukkur/24843 " data-dismiss="modal"
                                                style="color: #353944">
                                                Sukkur <span class="badge badge-gray-light pull-right">165</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="swabi" type="checkbox">
                                            <a href="/used-cars/swabi/24844 " data-dismiss="modal"
                                                style="color: #353944">
                                                Swabi <span class="badge badge-gray-light pull-right">314</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="swat" type="checkbox">
                                            <a href="/used-cars/swat/24860 " data-dismiss="modal"
                                                style="color: #353944">
                                                Swat <span class="badge badge-gray-light pull-right">38</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="talagang" type="checkbox">
                                            <a href="/used-cars/talagang/24847 " data-dismiss="modal"
                                                style="color: #353944">
                                                Talagang <span class="badge badge-gray-light pull-right">100</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="taxila" type="checkbox">
                                            <a href="/used-cars/taxila/24848 " data-dismiss="modal"
                                                style="color: #353944">
                                                Taxila <span class="badge badge-gray-light pull-right">148</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="toba-tek-singh" type="checkbox">
                                            <a href="/used-cars/toba-tek-singh/68123 " data-dismiss="modal"
                                                style="color: #353944">
                                                Toba Tek Singh <span
                                                    class="badge badge-gray-light pull-right">153</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="vehari" type="checkbox">
                                            <a href="/used-cars/vehari/24851 " data-dismiss="modal"
                                                style="color: #353944">
                                                Vehari <span class="badge badge-gray-light pull-right">158</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="wah-cantt" type="checkbox">
                                            <a href="/used-cars/wah-cantt/24852 " data-dismiss="modal"
                                                style="color: #353944">
                                                Wah cantt <span class="badge badge-gray-light pull-right">648</span>
                                            </a>
                                        </label>
                                    </li>
                                    <li>
                                        <label class="checkbox">
                                            <input value="wazirabad" type="checkbox">
                                            <a href="/used-cars/wazirabad/24853 " data-dismiss="modal"
                                                style="color: #353944">
                                                Wazirabad <span class="badge badge-gray-light pull-right">70</span>
                                            </a>
                                        </label>
                                    </li>
                                </ul>
                            </div>
                            <div class="modal-footer">
                                <button class="btn btn-link" type="button" value="submit"
                                    onclick="$('[name=city_list]').find('input').attr('checked', false);"> Clear
                                </button>
                                <div class="pull-right">
                                    <button class="btn btn-primary" type="button" value="submit"
                                        onclick="return doSubmitCities(this);">Submit</button>
                                </div>
                            </div>
                        </form>
                    </div>
                </div>

            </div>

        </div>
        <div id="Province">
            <div class="drop-down" data-bs-auto-close="false" data-bs-toggle="dropdown">
                Province

                <i class="fa-solid fa-caret-down"></i>
            </div>
            <div class="drop-down-menu">
                <div>
                    <ul class="dropdown-menu" aria-labelledby="Province">
                        <li>
                            <input type="checkbox">
                            Punjab
                            <span>18460</span>
                        </li>
                        <li>
                            <input type="checkbox">

                            sind
                            <span>18174</span>
                        </li>
                        <li>
                            <input type="checkbox">

                            kpk
                            <span>12949</span>
                        </li>
                        <li>
                            <input type="checkbox">

                            Balochistan

                            <span>5992</span>
                        </li>
                        <li>
                            <input type="checkbox">
                            Azad Kashmir
                            <span>4266</span>
                        </li>
                        <li>
                            <input type="checkbox">

                            Federally Administered Tribal Areas

                            <span>4266</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div id="Make">
            <div class="drop-down" data-bs-auto-close="false" data-bs-toggle="dropdown">
                Make
                <i class="fa-solid fa-caret-down"></i>
            </div>
            <div class="drop-down-menu">
                <div>
                    <ul class="dropdown-menu" aria-labelledby="Make">
                        <li>
                            <input type="checkbox">
                            Toyota
                            <span>18460</span>
                        </li>
                        <li>
                            <input type="checkbox">
                            Suzuki
                            <span>18174</span>
                        </li>
                        <li>
                            <input type="checkbox">
                            Honda
                            <span>12949</span>
                        </li>
                        <li>
                            <input type="checkbox">
                            Daihatsu
                            <span>5992</span>
                        </li>
                        <li>
                            <input type="checkbox">
                            KIA
                            <span>4266</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div id="Price-Range">
            <div class="drop-down" data-bs-auto-close="false" data-bs-toggle="dropdown">
                Price Range
                <i class="fa-solid fa-caret-down"></i>
            </div>
            <div class="dropdown-menu" aria-labelledby="Price">
                <div class="srch-bar">
                    <div class="srch-wrapper">
                        <input type="number" placeholder="From" id="Price-from">
                        <input type="number" placeholder="To" id="Price-to">
                        <span class="go-btn" @click="priceFilter">Go</span>
                    </div>
                </div>
            </div>
        </div>
        <div id="Year">
            <div class="drop-down" data-bs-auto-close="false" data-bs-toggle="dropdown">
                Year
                <i class="fa-solid fa-caret-down"></i>
            </div>
            <div class="dropdown-menu" aria-labelledby="Year">
                <div class="srch-bar">
                    <div class="srch-wrapper">
                        <input type="number" placeholder="From" id="year-from">
                        <input type="number" placeholder="To" id="year-to">
                        <span class="go-btn">Go</span>
                    </div>
                </div>
            </div>
        </div>

        <div id="Mileage">
            <div class="drop-down" data-bs-auto-close="false" data-bs-toggle="dropdown">
                Mileage (Km)
                <i class="fa-solid fa-caret-down"></i>
            </div>
            <div class="dropdown-menu" aria-labelledby="Mileage">
                <div class="srch-bar">
                    <div class="srch-wrapper">
                        <input type="text" placeholder="From" id="mileage-from">
                        <input type="text" placeholder="To" id="mileage-to">
                        <span class="go-btn">Go</span>
                    </div>
                </div>
            </div>
        </div>
        <div id="Registered">
            <div class="drop-down" data-bs-auto-close="false" data-bs-toggle="dropdown">
                Registered In

                <i class="fa-solid fa-caret-down"></i>
            </div>
            <div class="drop-down-menu">
                <div>
                    <ul class="dropdown-menu" aria-labelledby="Registered">
                        <li>
                            <input type="checkbox">
                            Punjab
                            <span>18460</span>
                        </li>
                        <li>
                            <input type="checkbox">

                            sind
                            <span>18174</span>
                        </li>
                        <li>
                            <input type="checkbox">

                            kpk
                            <span>12949</span>
                        </li>
                        <li>
                            <input type="checkbox">

                            Balochistan

                            <span>5992</span>
                        </li>
                        <li>
                            <input type="checkbox">
                            Azad Kashmir
                            <span>4266</span>
                        </li>
                        <li>
                            <input type="checkbox">

                            Federally Administered Tribal Areas

                            <span>4266</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>

    </div>
    <ul id="test">
        <li>12</li>
        <li>13</li>
        <li>14</li>
        <li>15</li>
    </ul>
</template>

<script>
export default {
    data() {
        return {
            filtered: {
                City: [],
                price: []

            },
        }
    },


    mounted() {
        this.cityFilter()

    },
    methods: {

        cityFilter() {

            let cities = document.querySelectorAll('#check-boxes input[type="checkbox"]')

            cities.forEach((item) => {
                item.addEventListener("change", () => {

                    this.$store.commit('filterData', this.filtered)
                    // console.log(this.$store.getters.getData)
                    this.$store.dispatch('checkBoxFilter', this.filtered)

                })
            })
        },
        priceFilter() {
            let from = document.querySelector('#check-boxes #Price-Range #Price-from').value
            let to = document.querySelector('#check-boxes #Price-Range #Price-to').value
            let price = {
                from,
                to
            }
            if (price.from !== '' && price.to !== '') {

                this.$store.dispatch('rangeFilter', price)
            }
            else {
                alert('please fill the value')
            }

        }

    }
}
</script>

<style>
#check-boxes .dropdown-menu {
    position: static !important;
    transform: none !important;
}

#check-boxes .dropdown-menu.show {
    border: none !important;
    padding: 10px 20px;
    background-color: white;
    font-size: 12px;
}

#check-boxes .dropdown-menu li {
    padding: 4px 0px;
}

#check-boxes .dropdown-menu li span {
    border: 1px solid #EAEDEF;
    float: right;
    border-radius: 10px;
    padding: 0px 5px;

}

#check-boxes .dropdown-menu li input {
    margin: 0px 3px;
}

#check-boxes .srch-wrapper input:nth-child(2) {
    border-left: 1px solid gainsboro;
}

.modal-header {
    display: block !important;
    padding: 15px;
    border-bottom: 1px solid #e6e6e6;
}

.modal-dialog {
    min-width: 32%;
    margin: 30px auto;
}

.modal .close {
    height: 26px;
    margin: 0;
    float: right;
    background: transparent;
    outline: none;
    border: none;
    font-size: 31px;
    display: flex;
    align-items: center;
}

.modal-body {
    overflow: auto;
    position: relative;
    padding: 15px;
}

.checkbox-list {
    max-height: 360px;
}

.list-links>li {
    width: 50%;
    padding: 0 10px;
    float: left;
}

.checkbox {
    position: relative;
    display: block !important;
    margin-top: 10px;
    margin-bottom: 10px;
    font-size: 12px;
}

.modal h4 {
    font-size: 14px;
    color: #233d7b;
    font-weight: 700;
}

.list-links .checkbox input {
    margin: 0;
    margin-right: 5px;
    position: relative;
    vertical-align: -2px;
}

.badge-gray-light {
    font-size: 11px;
    background: #dedede;
    color: #27324e !important;
    font-weight: normal;
}

.pull-right {
    float: right !important;
}

.badge {

    min-width: 10px;
    padding: 3px 7px;
    font-size: 12px;
    font-weight: bold;
    color: #000;
    line-height: 1;
    vertical-align: middle;
    white-space: nowrap;
    text-align: center;
    border-radius: 10px;

}
#test li::-ms-check{
    background: red;
    width: 50px;
}
</style>
