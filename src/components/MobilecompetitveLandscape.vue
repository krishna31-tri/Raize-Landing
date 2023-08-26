<template>
    <div class="mobile-comp">
        <h2>Competitive landscape</h2>
        <p>Short description goes here</p>
        <div class="mobile-comp-div">
            <ul class="mobile-comp-static">
                <li>Free Access</li>
                <li>Access without Token and Lock</li>
                <li>Investment Size (>1k)</li>
                <li>Referral System (Lifetime)</li>
                <li>seed</li>
                <li>Type of Deal Private</li>
                <li>Public</li>
                <li>Lottery (Basic)</li>
                <li>FCFS (Genesis)</li>
                <li>Equity Deals</li>
            </ul>
            <swiper class="custom-swiper" :modules="modules" :slides-per-view="2" :space-between="0" navigation
                :pagination="{ clickable: true }" :scrollbar="{ draggable: true }" @swiper="onSwiper"
                @slideChange="onSlideChange">
                <swiper-slide class="slide">
                    <ul class="mobile-comp-dynamic">
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                    </ul>
                </swiper-slide>
                <swiper-slide class="slide">
                    <ul class="mobile-comp-dynamic">
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>❌</li>
                        <li>❌</li>
                        <li>✔️</li>
                        <li>❌</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>❌</li>
                        <li>❌</li>
                    </ul>
                </swiper-slide>
                <swiper-slide class="slide">
                    <ul class="mobile-comp-dynamic">
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                    </ul>
                </swiper-slide>
                <swiper-slide class="slide">
                    <ul class="mobile-comp-dynamic">
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                    </ul>
                </swiper-slide>
                <swiper-slide class="slide">
                    <ul class="mobile-comp-dynamic">
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                        <li>✔️</li>
                    </ul>
                </swiper-slide>
            </swiper>
        </div>

    </div>
</template>
<script>
// import Swiper core and required modules
import { Navigation, Pagination, Scrollbar, A11y } from 'swiper/modules';

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/navigation';
import 'swiper/css/pagination';
import 'swiper/css/scrollbar';

// Import Swiper styles
export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    setup() {
        const onSwiper = (swiper) => {
            console.log(swiper);
        };
        const onSlideChange = () => {
            console.log('slide change');
        };
        return {
            onSwiper,
            onSlideChange,
            modules: [Navigation, Pagination, Scrollbar, A11y],
        };
    },
};
</script>
<style>
.mobile-comp {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.mobile-comp-div {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 14%;
}

.slide {
    border-right: 1px solid #4A71F0;
    border-left: 1px solid #4A71F0;
    width: 100px;
}

.mobile-comp li {
    list-style: none;
    height: 55px;
    color: #4A71F0;
    text-align: start;
    font-weight: 600;
    padding-left: 6%;
}

.mobile-comp-static {
    width: 50%;
}

.custom-swiper {
    width: 200px;
    margin: 0;
    overflow: clip;
    overflow-y: visible;
}

.swiper-button-prev,
.swiper-button-next {
    top: -1%;
    width: 20px;
    height: 20px;
    z-index: 15;
}

.swiper-pagination-fraction,
.swiper-pagination-custom,
.swiper-horizontal>.swiper-pagination-bullets,
.swiper-pagination-bullets.swiper-pagination-horizontal {
    top: -6%;
}

.swiper-button-prev::after,
.swiper-button-next::after {
    width: 20px;
    height: 20px;
    font-size: 20px;
}

.swiper-horizontal>.swiper-scrollbar,
.swiper-scrollbar.swiper-scrollbar-horizontal {
    display: none;
}

@media (min-width:768px) {
    .mobile-comp {
        display: none;
    }
}
</style>