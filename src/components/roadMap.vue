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
                        <h2>Event 2</h2>
                        <p>Event 2 description</p>
                    </div>

                </div>
                <div className="timeline-item">
                    <div className="circle"></div>
                    <div className="timeline-content">
                        <h2>Event 2</h2>
                        <p>Event 2 description</p>
                    </div>

                </div>
                <div className="timeline-item">
                    <div className="circle"></div>
                    <div className="timeline-content">
                        <h2>Event 2</h2>
                        <p>Event 2 description</p>
                    </div>

                </div>
                <div className="timeline-item">
                    <div className="circle"></div>
                    <div className="timeline-content">
                        <h2>Event 2</h2>
                        <p>Event 2 description</p>
                    </div>

                </div>
                <div className="timeline-item">
                    <div className="circle"></div>
                    <div className="timeline-content">
                        <h2>Event 2</h2>
                        <p>Event 2 description</p>
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
}

.roadmapbg {
    position: absolute;
    top: 0%;
    left: 0%;
    width: 100%;
    height: 100%;
    z-index: -1;
}

.timeline {
    position: relative;
    max-width: 800px;
    margin: 2% auto;
    padding: 20px;
    color: black;
    width: 80%;
}

.timeline::before {
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0%;
    width: 9px;
    background-color: #838383;
    transform: translateX(-50%);
}


.timeline-item {
    position: relative;
    margin-bottom: 50px;
    margin-left: 22px;
}

.timeline-content {
    background-color: transparent;
    padding: 20px;
    border-radius: 4px;
    color: black;
    border: 2px solid black;

    margin-bottom: 10px;

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
    left: -53px;
    top: 94px;
    margin-bottom: 20px;
    z-index: 2;
    border: 2px solid black;
}

@media (min-width:1000px) {
    .roadmap {
        display: none;
    }
}
</style>
  