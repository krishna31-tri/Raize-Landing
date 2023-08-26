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
                <div class="menu-content">
                    <ul class="menu-items">
                        <li><a href="#">Compliant</a></li>
                        <li><a href="#">FAQ</a></li>
                        <li><a href="#">Security Sauce</a></li>
                        <li><a href="#">Pricing</a></li>
                        <li><a href="#">Launch</a></li>
                        <li><a href="mailto:contact@example.com">Email</a></li>
                    </ul>
                    <div class="menu-buttons">
                        <button class="launch-button">Launch Now</button>
                        <div class="get-in-touch">
                            <p>Get in touch!</p>
                            <a class="email-link" href="mailto:hello@raizerpartner.com">hello@raizerpartner.com</a>
                        </div>
                    </div>
                </div>
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
.menu-content{
    display: flex;
    justify-content: space-around;
    margin-top: 95px;
    /* gap: 241px; */
    flex-direction: row;
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

/* Rest of your styles... */
.row {
    display: flex;
    align-items: center;
}

/* Adjust spacing as needed */
.column {
    margin-right: 20px;
}
.menu-items {
    list-style: none;
    padding: 0;
    display: flex;
    margin: 0;
    gap: 24px;
    text-align: left;
    flex-direction: column;
}

.menu-items li {
    margin-bottom: 15px;
}

.menu-items li a {
    text-decoration: none;
    /* color: #333; */
    font-weight: bold;
    font-size: 16px;
    transition: color 0.3s;
    color: rgba(110, 116, 128, 1);
    font-family: 'Plus Jakarta Sans';
}


.menu-buttons {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: flex-end;
}

.launch-button,
.contact-button {
    height: 44px;
    width: 140px;
    border-radius: 60px;
    padding: 10px 20px;
    background: rgba(74, 113, 240, 1);
    font-weight: 500;
    /* margin-right: 10px; */
    font-size: 16px;
    border: none;
    /* border-radius: 5px; */
    /* background-color: #ff9900; */
    color: #fff;
    cursor: pointer;
}
.get-in-touch {
    padding: 20px;
    text-align: right;
    font-size: 16px;
    font-family: 'plus Jakarta Sans';
}

.get-in-touch p {
  font-size: 18px;
  margin-bottom: 10px;
}

.email-link {
    display: inline-block;
    font-size: 16px;
    color: blue;
    text-decoration: none;
    font-weight: 700;
}
.launch-button:hover,
.contact-button:hover {
    background-color: #e67e00;
}
</style>
