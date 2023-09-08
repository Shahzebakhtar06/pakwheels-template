<template>
    <div class="app-install-banner-wrapper">
        <div class="container bg-wrapper">
            <div class="row">
                <div class="col-md-9">
                    <div class="row d-flex align-center">
                        <div class="col-md-8 ps-0">
                            <h2 class="fs28 text-primary mb-3">Get The PakWheels App</h2>
                            <p class="mt-3 fs16 mb-5">Buy &amp; Sell Cars, Bikes and Auto Parts faster and better <br>
                                using our App</p>
                            <a href="https://play.google.com/store/apps/details?id=com.pakwheels&amp;referrer=utm_source%3Dpakwheels.com%26utm_medium%3Dweb-link%26utm_content%3Dfooter%26utm_campaign%3Dorganic-installs"
                                onclick="trackEvents('User', 'FromBanner - AppInstallClicked', 'GooglePlay');"
                                target="_blank" title="PakWheels Android App"><img alt="Google-play-badge" height="40"
                                    loading="lazy"
                                    src="https://wsa4.pakwheels.com/assets/google-play-badge-f4bed6cbd8a3a1be7c79377c4441447a.svg"></a>
                            <a href="https://click.google-analytics.com/redirect?tid=UA-642162-19&amp;url=https%3A%2F%2Fitunes.apple.com%2Fpk%2Fapp%2Fpakwheels%2Fid739776365%3Fmt%3D8&amp;aid=com.pakwheels.www&amp;idfa={idfa}&amp;cs=pakwheels.com&amp;cm=web-link&amp;cn=organic-installs&amp;cc=footer&amp;hash=md5"
                                onclick="trackEvents('User', 'FromBanner - AppInstallClicked', 'AppStore');"
                                style="margin: 0px 3px" target="_blank" title="PakWheels iOS App"><img
                                    alt="App-store-badge" height="40" loading="lazy"
                                    src="https://wsa1.pakwheels.com/assets/app-store-badge-4d05ff70e5546f31e3891739ea40abad.svg"></a>
                            <a href="https://appgallery.huawei.com/#/app/C101437147"
                                onclick="trackEvents('User', 'FromBanner - AppInstallClicked', 'AppGallery');"
                                target="_blank" title="PakWheels Android App"><img alt="Huawei-store-badge" height="40"
                                    loading="lazy"
                                    src="https://wsa4.pakwheels.com/assets/huawei-store-badge-7ad06f9ffe74b644d49c6221af98f5b3.svg"></a>
                        </div>
                        <div class="col-md-4 col-md-offset-1">
                            <div class="qr-code-cont">
                                <img alt="Scanner_arrow" class="qr-code-arrow"
                                    src="https://wsa4.pakwheels.com/assets/promotion-app/scanner_arrow-e49b64a6868f7f501b191d7b984c4268.svg">
                                <img alt="App-install-qr-code" class="mr15"
                                    src="https://wsa3.pakwheels.com/assets/promotion-app/app-install-qr-code-281c1dc2396c1735eadfe5f80c020673.svg">
                                <p class="mb-0">Scan the QR<br> to get the App</p>
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

}
</script>

<style>
.app-install-banner-wrapper .bg-wrapper {
    padding: 15px 10px 35px !important;
    background: url(../../public/app-banner.png) no-repeat right bottom;
    background-size: contain;

}

.fs28 {
    font-size: 28px;
}

h2.text-primary {
    color: #233d7b !important;
    font-weight: 800;
}
.app-install-banner-wrapper{
    color: #7b8397;

}
hr {
    margin-top: 20px;
    margin-bottom: 20px;
    border: 0;
    border-top: 1px solid rgb(212 210 210) !important;
}
.qr-code-cont {
    display: flex;
    align-items: center;
    position: relative;
}

.qr-code-cont .qr-code-arrow {
    position: absolute;
    top: -6px;
    left: 74px;
    z-index: 1;
}
</style>