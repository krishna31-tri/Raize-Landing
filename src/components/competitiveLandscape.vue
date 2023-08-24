<template>
  <div class="table-container">
    <h1>Competitive Landscape</h1>
    <table class="custom-table">
      <thead>
        <tr>
          <th style="width: 200px; background: none;"></th>
          <th v-for="(company, companyName) in companies" :key="companyName" style="width: 200px; background: none;">{{ companyName }}</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(property, propertyName) in properties" :key="propertyName">
          <td>{{ propertyName }}</td>
          <td v-for="(company, companyName) in companies" :key="companyName">
              {{ getTickCross(company[propertyName]) }}
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      companies: {
        Raize: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          typeOfDeal: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        abv: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          typeOfDeal: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        ccc: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          typeOfDeal: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        sss: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          typeOfDeal: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        dds: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          typeOfDeal: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        sa: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          typeOfDeal: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        // Add other companies and their properties here
      },
      properties: {
        "Free Access": "freeAccess",
        "Access without Token and Lock": "accessWithoutTokenAndLock",
        "Investment Size (>1k)": "investmentSize",
        "Referral System (Lifetime)": "referralSystem",
        "Type of Deal": "typeOfDeal",
        "Lottery (Basic)": "lottery",
        "FCFS (Genesis)": "fcfs",
        "Equity Deals": "equityDeals",
      },
    };
  },
  methods: {
    getTickCross(value) {
      return value ? "✔️" : "❌";
    },
  },
};
</script>
<style scoped>
.table-container {
  display: flex;
    align-items: center;
    margin-top: 20px;
    flex-direction: column;
}

.custom-table {
  border-collapse: collapse;
  width: 80%;
  border: none;
}

.custom-table th,
.custom-table td {
  border: none;
  padding: 10px;
  text-align: center;
  border-right: 1px solid blue;
}

.custom-table th:first-child,
.custom-table td:first-child {
  text-align: left;
  border-left: none;
}

.custom-table th {
  font-weight: bold;
}

.custom-table td {
  font-size: 16px;
}

.tick {
  color: green;
}

.cross {
  color: red;
}

.highlighted-row {
  background-color: rgba(0, 180, 215, 0.37);
}
</style>