<template>
    <div class="roadmap">
        <img class="roadmapbg" alt="Vue logo" src="../assets/roadmapbg.svg" />
        <div class="roadmap-div">
            <h1>Road Map</h1>
            <p>Short description goes here</p>

            <div className="timeline">
                <div className="timeline-item">
                    <div className="circle"></div>
                    <div className="timeline-content">
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
                    </div>

                </div>
                <div className="timeline-item">
                    <div className="circle"></div>
                    <div className="timeline-content">
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
                    </div>

                </div>
                <div className="timeline-item">
                    <div className="circle"></div>
                    <div className="timeline-content">
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
                    </div>

                </div>
                <div className="timeline-item">
                    <div className="circle"></div>
                    <div className="timeline-content">
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
                    </div>

                </div>
                <div className="timeline-item">
                    <div className="circle"></div>
                    <div className="timeline-content">
                        <h2>Q4 -2024</h2>
                        <ul>
                            <li>OTC deals marketplace</li>
                            <li>V.3 Queue</li>
                            <li>V.2 Growth Hacking</li>
                            <li>functionalities</li>
                            <li>V.3 Referral</li>
                            <li>DEX Integration</li>
                        </ul>
                    </div>

                </div>

            </div>
        </div>
    </div>
</template>
  
<script>

</script>
  
<style scoped>
.roadmap {
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

.roadmap-div h1 {
    width: 100vw;
    text-align: center;
}

.timeline {
    position: relative;
    max-width: 800px;
    margin: 2% auto;
    padding: 20px;
    width: 80%;
    z-index: 3;
}

.timeline::before {
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0%;
    width: 9px;
    background-color: #A3B8FA;
    transform: translateX(-50%);
}


.timeline-item {
    position: relative;
    margin-bottom: 50px;
    margin-left: 22px;
    z-index: 3;
}

.timeline-content {
    flex: 1;
    padding: 20px;
    text-align: center;
    position: relative;
    border: 2px solid #4A71F0;
    max-width: 80%;
    border-radius: 8px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: self-start;
    background-color: #fff;


}

.timeline-content ul {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
}

.timeline-content li {
    list-style: disc;
    text-align: start;
    margin: 2px;
}

.timeline p {
    text-align: start;
}

.timeline .circle {
    width: 20px;
    height: 20px;
    border-radius: 100%;
    background-color: #004ef7;
    position: relative;
    left: -52px;
    top: 94px;
    margin-bottom: 20px;
    z-index: 2;
}

@media (min-width:1188px) {
    .roadmap {
        display: none;
    }
}
</style>