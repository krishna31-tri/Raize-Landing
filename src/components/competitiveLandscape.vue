<template>
  <div class="table-container">
    <h1>Competitive Landscape</h1>
    <p>Short description goes here</p>
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
            {{ getTickCross(company[properties[propertyName]]) }}
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
          seed: true,
          typeOfDeal: true,
          public: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        Coinlist: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          seed: true,
          typeOfDeal: true,
          public: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        Republic: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          seed: false,
          typeOfDeal: true,
          public: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        DAOMaker: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          seed: false,
          typeOfDeal: true,
          public: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
        Tokensoft: {
          freeAccess: true,
          accessWithoutTokenAndLock: false,
          investmentSize: true,
          referralSystem: false,
          seed: false,
          typeOfDeal: true,
          public: true,
          lottery: true,
          fcfs: false,
          equityDeals: true,
        },
      },
      properties: {
        "Free Access": "freeAccess",
        "Access without Token and Lock": "accessWithoutTokenAndLock",
        "Investment Size (>1k)": "investmentSize",
        "Referral System (Lifetime)": "referralSystem",
        "seed": "seed",
        "Type of Deal Private": "typeOfDeal",
        "Public": "public",
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
  flex-direction: column;
  width: 80%;
  margin: 5% auto;
}

.table-container h1 {
  margin: 0;
}

.custom-table {
  border-collapse: collapse;
  width: 80%;
  border: none;
  margin-top: 2%;
}

.custom-table th,
.custom-table td {
  border: none;
  padding: 10px;
  text-align: center;
  border-right: 1px solid blue;
}

.custom-table th {
  border: none;
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
