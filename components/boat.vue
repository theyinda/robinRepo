<template>
  <section class="dashboard-view">
    <div class="table-container">
      <div class="chat">
        <div>
          <p>Conversations <span class="num">54</span></p>
        </div>
        <div class="search">
          <input class="" placeholder="Search Chat" />
          <img src="../assets/images/icon.svg" alt="icon" class="search-icon" />
        </div>
      </div>
      <table>
        <thead>
          <tr class="table-header">
            <th>Token</th>
            <th>Created On</th>
            <th>Last Meeting On</th>
            <th>Message Count</th>
          </tr>
        </thead>

        <tr
          v-for="records in tableData"
          :key="records.token"
          class="table-body"
        >
          <td class="code">{{ records.token }}</td>
          <td class="">{{ records.created }}</td>
          <td class="">{{ records.meeting }}</td>
          <td class="">{{ records.message }}</td>
        </tr>
      </table>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      tableData: [
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
        {
          token: 'Ukssda12sa...',
          created: 'Tuesday, Dec 8th 2021',
          meeting: 'Tuesday, Dec 8th 2021',
          message: '9261',
        },
      ],
    }
  },
}
</script>

<style>
.container {
  display: flex;
  max-width: 1448px;
}
.dashboard-view {
  width: 1079px;
}
.dashboard-view-container {
  background: #ffffff;
  box-shadow: 0px -7px 24px rgba(0, 0, 0, 0.25);
  padding: 20px 20px;
}

.table-container {
  width: 95%;
  margin: 10px auto;
  background: #fff;
}
table {
  border-spacing: 0px;
  width: 100%;
  box-shadow: 0px 4px 4px rgba(86, 107, 160, 0.05);
  border-radius: 5px;
}

.table-header {
  width: 10%;
  text-align: center;
}

/* tr:nth-of-type(even) {
  background-color: #f5f5f5;
} */
td {
  padding: 15px 25px 15px 40px;
  width: 10%;
  text-align: center;
  font-size: 12px;
  line-height: 15px;
  color: #566ba0;
  border-bottom: 1px solid #000000;
}
th {
  /* padding: 15px 23px 15px 0px; */
  padding: 15px 0;
  width: 10%;
  text-align: center;
  font-size: 14px;
  line-height: 17px;
  font-weight: normal;
  color: #566ba0;
  border-bottom: 1px solid #000000;
}
.chat {
  display: flex;
  justify-content: space-between;
  /* background: yellow; */
  width: 100%;
  margin-top: 90px;
  border-bottom: 1px solid #000000;
}
.chat p {
  padding: 15px 0 0 23px;
}

.chat input {
  background: #ffffff;
  opacity: 0.54;
  border: 1px solid #c1cec8;
  border-radius: 10px;
  width: 269px;
  padding: 10px 15px;
  margin-top: 20px;
  margin-right: 30px;
}
.code {
  color: #14865a;
  opacity: 0.9;
}
.num {
  opacity: 0.3;
}
.search {
  position: relative;
}
.search-icon {
  position: absolute;
  top: 30px;
  right: 45px;
  cursor: pointer;
}
</style>
