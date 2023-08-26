<template>
    <div class="roadmap-desktop">
        <img class="roadmapbg" alt="Vue logo" src="../assets/roadmapbgdesktop.svg" />
        <div class="timeline">
            <h1>Road Map</h1>
            <p>Short description goes here</p>
            <div class="upper-components">
                <div class="event" id="ev1">
                    <h2>Q4 - 2023</h2>
                    <ul>
                        <li>Genesis pre-sale</li>
                        <li>Genesis sales</li>
                        <li>Launch marketing campaign</li>
                        <li>Beta launch/ test</li>
                        <li>First private deals listing for genesis</li>
                        <li>V.1 Referral program</li>
                        <li>V.1 website</li>
                    </ul>
                    <div class="vert-line" id="vl1"></div>
                    <div class="circles" id="c1">

                    </div>
                </div>
                <div class="event">
                    <h2>Q1 - 2024</h2>
                    <ul>
                        <li>Surprise #1</li>
                        <li>V.2 Website</li>
                        <li>Launch V.1 App</li>
                        <li>Main Marketing ampaign Launch</li>
                        <li>Public deals launch</li>
                        <li>V.1 Queue functionalities</li>
                        <li>Partnerships</li>
                    </ul>
                    <div class="vert-line"></div>
                    <div class="circles">

                    </div>
                </div>
                <div class="event">
                    <h2>Q2 - 2024</h2>
                    <ul>
                        <li>V.1 Growth Hacking</li>
                        <li>functionalities</li>
                        <li>V.2 Referral program</li>
                        <li>Equity Deals Legal</li>
                        <li>investigation</li>
                        <li>OTC Deals Legal</li>
                        <li>Investigation</li>
                    </ul>
                    <div class="vert-line"></div>
                    <div class="circles">

                    </div>
                </div>
            </div>
            <div class="line4"></div>
            <div class="lower-components">
                <div class="event">
                    <h2>Q3 - 2024</h2>
                    <ul>
                        <li>Surprise #2</li>
                        <li>V.3 website</li>
                        <li>V.2 App</li>
                        <li>Equity deals</li>
                        <li>V.2 Queue</li>
                        <li>functionalities</li>
                        <li>On Ramp Integration</li>
                    </ul>
                    <div class="vert-line"></div>
                    <div class="circles">

                    </div>
                </div>
                <div class="event">
                    <h2>Q4 -2024</h2>
                    <ul>
                        <li>OTC deals marketplace</li>
                        <li>V.3 Queue</li>
                        <li>V.2 Growth Hacking</li>
                        <li>functionalities</li>
                        <li>V.3 Referral</li>
                        <li>DEX Integration</li>
                    </ul>
                    <div class="vert-line"></div>
                    <div class="circles">

                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    name: "TimelineComponent",
};
</script>
  
<style scoped>
.roadmap-desktop {
    text-align: center;
    position: relative;
    background-color: #F0F5FA;
}

.roadmapbg {
    position: absolute;
    top: 0%;
    left: 0%;
    width: 100%;
    height: 100%;
    z-index: 1;
}

.timeline {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    position: relative;
    padding-top: 50px;
}

.timeline h1 {
    margin: 0;
}

.line4 {
    width: 100%;
    height: 2px;
    background-color: #ccc;
    margin: 22px 0%;
    z-index: 2;
}

.upper-components {
    display: flex;
    justify-content: space-between;
    width: 80%;
    padding: 20px;
    max-width: 1500px;
    position: relative;
}

.lower-components {
    display: flex;
    justify-content: space-around;
    width: 80%;
    padding: 20px;
    max-width: 1500px;
    position: relative;
}

.upper-components .vert-line {
    height: 45px;
    width: 3px;
    position: absolute;
    left: 50%;
    bottom: -13%;
    z-index: 2;
    background-color: #30B6D2;
}

#vl1 {
    height: 25px;
    width: 3px;
    position: absolute;
    left: 50%;
    bottom: -8%;
}

#c1 {
    height: 23px;
    width: 23px;
    position: absolute;
    left: 46.5%;
    top: 104%;
    z-index: 2;
}



.upper-components .circles {
    height: 17px;
    width: 17px;
    position: absolute;
    left: 47.5%;
    top: 110%;
    z-index: 2;
    background-color: #4A71F0;
    border-radius: 100%;
    z-index: 4;

}

.lower-components .circles {
    height: 17px;
    width: 17px;
    position: absolute;
    left: 47.5%;
    top: -18%;
    z-index: 2;
    background-color: #4A71F0;
    border-radius: 100%;
    z-index: 4;
}

.lower-components .vert-line {
    height: 42px;
    width: 3px;
    position: absolute;
    left: 50%;
    top: -14%;
    z-index: 2;
    background-color: #30B6D2;
}

.event {
    flex: 1;
    padding: 20px;
    text-align: center;
    position: relative;
    border: 2px solid #4A71F0;
    max-width: 252px;
    border-radius: 8px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: self-start;
    background-color: #fff;
    z-index: 3;
}

#ev1 {
    border: 3px solid #4A71F0;
    scale: 1.1;
}

.event ul {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
}

.event li {
    list-style: disc;
    text-align: start;
    margin: 2px;
}


@media (max-width: 1188px) {
    .roadmap-desktop {
        display: none;
    }
}
</style>
  