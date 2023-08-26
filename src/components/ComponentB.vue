<template>
    <div class="component-b">
        <p class="free-text">$500<span class="lifetime-text">/ Lifetime</span></p>
        <p style="font-size: 12px; font-weight: 500; color: rgba(145,145,163,1);">One single payment. No more!</p>
        <button class="subscribe-button">Subscribe</button>
        <table class="properties">
            <tbody>
                <tr class="row">
                    <td>Platform Fee</td>
                    <td>10%</td>
                </tr>
                <tr class="row">
                    <td>Referral Award</td>
                    <td>0%</td>
                </tr>
                <tr class="row">
                    <td>1st Level</td>
                    <td>20%</td>
                </tr>
                <tr class="row">
                    <td>2nd Level</td>
                    <td>10%</td>
                </tr>
                <tr class="row">
                    <td>3rd Level</td>
                    <td>5%</td>
                </tr>
                <tr class="row">
                    <td>OTC Deals</td>
                    <td>_</td>
                </tr>
                <tr class="row">
                    <td>Investment Priority</td>
                    <td>FCFS</td>
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
    name: 'ComponentB',
};
</script>
  
<style scoped>
.component-b {
    background-color: #ffffff;
    padding: 20px 0px;
    border-radius: 5px;
}

.component-b tr:nth-child(odd) {
    background-color: #F0F5FA;
}

.component-b .properties {
    display: flex;
    justify-content: center;
    margin-top: 20px;
    align-items: center;

}

.component-b td {
    width: 50vw;
    padding: 3%;
    margin: 0;
}

.component-b td:first-child {
    color: #4A71F0;
    font-weight: 600;
}
</style>
  