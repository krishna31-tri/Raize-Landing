<template>
    <div class="toggle-container">
        <button class="toggle-button" @click="toggleComponent">
            <span :class="{ active: activeComponent === 'ComponentA' }">Basic</span>
            <span :class="{ active: activeComponent === 'ComponentB' }">Genesis</span>
        </button>
        <transition name="slide" mode="out-in">
            <component :is="activeComponent"></component>
        </transition>
    </div>
</template>
  
<script>
import ComponentA from './ComponentA.vue';
import ComponentB from './ComponentB.vue';

export default {
    components: {
        ComponentA,
        ComponentB,
    },
    data() {
        return {
            activeComponent: 'ComponentA',
        };
    },
    methods: {
        toggleComponent() {
            this.activeComponent = this.activeComponent === 'ComponentA' ? 'ComponentB' : 'ComponentA';
        },
    },
};
</script>
  
<style>
.toggle-container {
    text-align: center;
    margin-top: 20px;
}

.toggle-button {
    display: inline-block;
    background: #DAE2FA;
    color: #6E7480;
    border: none;
    padding: 15px 7px;
    cursor: pointer;
    border-radius: 60px;
    font-size: 16px;
    font-weight: bold;
}

.toggle-button span {
    margin: 0 5px;
}

.active {
    background: #fff;
    color: #4A71F0;
    padding: 10px 22px;
    border-radius: 5px;
    border-radius: 60px;
}

.slide-enter-active,
.slide-leave-active {
    transition: transform 0.5s cubic-bezier(0.55, 0.085, 0.68, 0.53);
}

.slide-enter,
.slide-leave-to {
    transform: translateX(100%);
}

.active-enter-active,
.active-leave-active {
    transition: background-color 0.3s ease-in-out, color 0.3s ease-in-out;
}

.active-enter,
.active-leave-to {
    background-color: #007bff;
    color: white;
}
</style>
  