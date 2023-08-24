<template>
    <div class="roadmap-desktop">
        <img class="roadmapbg" alt="Vue logo" src="../assets/roadmapbgdesktop.svg" />
        <div class="timeline">
            <div class="upper-components">
                <div class="event">
                    <h2>Component 1</h2>
                    <p>Description of Component 1</p>
                    <div class="vert-line"></div>
                </div>
                <div class="event">
                    <h2>Component 2</h2>
                    <p>Description of Component 2</p>
                    <div class="vert-line"></div>
                </div>
                <div class="event">
                    <h2>Component 3</h2>
                    <p>Description of Component 3</p>
                    <div class="vert-line"></div>
                </div>
            </div>
            <div class="line4"></div>
            <div class="lower-components">
                <div class="event">
                    <h2>Component 4</h2>
                    <p>Description of Component 4</p>
                    <div class="vert-line"></div>
                </div>
                <div class="event">
                    <h2>Component 5</h2>
                    <p>Description of Component 5</p>
                    <div class="vert-line"></div>
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
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    position: relative;
    padding-top: 50px;
}

.line4 {
    width: 100%;
    height: 2px;
    background-color: #ccc;
    margin: 3% 0%;
}

.upper-components {
    display: flex;
    justify-content: space-between;
    width: 80%;
    padding: 20px;
    max-width: 1500px;
}

.lower-components {
    display: flex;
    justify-content: space-around;
    width: 80%;
    padding: 20px;
    max-width: 1500px;
}

.upper-components .vert-line {
    height: 79px;
    width: 3px;
    position: absolute;
    left: 50%;
    bottom: -64%;
    z-index: 2;
    background-color: red;
}

.lower-components .vert-line {
    height: 79px;
    width: 3px;
    position: absolute;
    left: 50%;
    top: -64%;
    z-index: 2;
    background-color: red;
}

.event {
    flex: 1;
    padding: 20px;
    text-align: center;
    position: relative;
    border: 2px solid red;
    max-width: 25%;
}

@media (max-width: 768px) {
    .roadmap-desktop {
        display: none;
    }
}
</style>
  