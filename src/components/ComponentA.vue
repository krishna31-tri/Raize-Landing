<template>
    <div class="component-a">
        <p class="free-text">Free<span class="lifetime-text">/Lifetime</span></p>
        <p style="font-size: 12px; font-weight: 500; color: rgba(145,145,163,1);">Free of charge. Start Anytime</p>
        <button class="signUp-button">Sign Up</button>
        <table class="properties">
            <tbody>
                <tr class="row">
                    <td>Platform Fee</td>
                    <td>20%</td>
                </tr>
                <tr class="row">
                    <td>Referral Award</td>
                    <td>0%</td>
                </tr>
                <tr class="row">
                    <td>1st Level</td>
                    <td>5%</td>
                </tr>
                <tr class="row">
                    <td>2nd Level</td>
                    <td>_</td>
                </tr>
                <tr class="row">
                    <td>3rd Level</td>
                    <td>_</td>
                </tr>
                <tr class="row">
                    <td>OTC Deals</td>
                    <td>_</td>
                </tr>
                <tr class="row">
                    <td>Investment Priority</td>
                    <td>Lottery</td>
                </tr>
                <tr class="row">
                    <td>Private Deals</td>
                    <td>_</td>
                </tr>
                <tr class="row">
                    <td>Equity Deals</td>
                    <td>_</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>
  
<script>
export default {
    name: 'ComponentA',
};
</script>
  
<style scoped>
.component-a {
    background-color: #ffffff;
    padding: 20px 0px;
    border-radius: 5px;
}

.component-a tr:nth-child(odd) {
    background-color: #F0F5FA;
}

.component-a .properties {
    display: flex;
    justify-content: center;
    margin-top: 20px;
    align-items: center;

}

.component-a td {
    width: 50vw;
    padding: 3%;
    margin: 0;
}

.component-a td:first-child {
    color: #4A71F0;
    font-weight: 600;
}
</style>
  