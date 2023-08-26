<template>
    <div class="mobile-nav">
        <div class="logo">
            <img alt="Vue logo" src="../assets/raiseLogo.png">
        </div>
        <div class="nav-toggle" @click="toggleMenu">
            <div class="icon" :class="{ 'open': showMenu }">
                <div class="bar"></div>
                <div class="bar"></div>
                <div class="bar"></div>
            </div>
        </div>
        <transition name="slide">
            <div v-if="showMenu" class="menu">
                <!-- Your menu content here -->
            </div>
        </transition>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            showMenu: false,
        };
    },
    methods: {
        toggleMenu() {
            this.showMenu = !this.showMenu;
        },
    },
};
</script>
  
<style scoped>
.mobile-nav {
    position: fixed;
    top: 0px;
    left: 0px;
    display: flex;
    align-items: center;
    z-index: 1000;
    justify-content: space-between;
    align-items: center;
    width: 95vw;
    margin: auto;
    padding: 2vw 3vw;
}

.logo {
    margin-right: auto;
    /* Add styles to position and size your logo */
}

.nav-toggle {
    width: 40px;
    height: 40px;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
}

.icon {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    width: 20px;
    height: 16px;
}

.bar {
    width: 20px;
    height: 2px;
    background-color: #333;
    transition: transform 0.3s, opacity 0.3s;
}

.open .bar:nth-child(1) {
    transform: translateY(6px) rotate(45deg);
}

.open .bar:nth-child(2) {
    opacity: 0;
}

.open .bar:nth-child(3) {
    transform: translateY(-6px) rotate(-45deg);
}

.menu {
    position: absolute;
    top: 0px;
    right: 0;
    width: 100vw;
    height: 100vh;
    background-color: #fff;
    box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.1);
    padding: 20px;
    border-radius: 5px;
    animation: slide-in-3cbfc4a1 0.3s ease;
    z-index: -1;
}

@keyframes slide-in {
    from {
        transform: translateX(100%);
    }

    to {
        transform: translateX(0);
    }
}

@media(min-width:1100px) {
    .mobile-nav {
        display: none;
    }
}
</style>
  