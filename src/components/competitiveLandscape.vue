<template>
  <div class="table-container">
    <h1>Competitive Landscape</h1>
    <table class="custom-table">
      <thead>
        <tr>
          <th style="width: 200px; background: none;"></th>
          <th v-for="(company, companyName) in companies" :key="companyName" style="width: 200px; background: none;">
            <img :src="getCompanyLogo(companyName)" alt="Company Logo" class="company-logo" />
          </th>
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
      // ... your companies and properties data ...
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
        Coinlist: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          typeOfDeal: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        Republic: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          typeOfDeal: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        DAOMaker: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          typeOfDeal: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        Tokensoft: {
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
    getCompanyLogo(companyName) {
      // Adjust this path based on your actual project structure
      return require(`@/assets/${companyName}_logo.png`);
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
  color: rgba(74, 113, 240, 1);
  border-left: none;
  font-size: 16px;
  font-family: 'Plus Jakarta Sans';
  font-weight: 700;
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

.company-logo {
  max-width: 100px;
  max-height: 40px;
}

@media (max-width:768px) {
  .table-container {
    display: none;
  }
}
</style>
