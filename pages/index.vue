<template>
  <div class="container">
    <div class="sidebar">
      <nav class="sidebar">
        <div class="logo">
          <img src="../assets/images/logo.svg" class="logo" alt="logo" />
        </div>
        <nuxt-link to="/"
          ><div class="side-nav_item">
            <img src="../assets/images/dashboard.svg" alt="icon" />
            <p>Dashboard</p>
          </div></nuxt-link
        >

        <nuxt-link to="/chat"
          ><div class="side-nav_item">
            <img src="../assets/images/chat.svg" alt="icon" />
            <p>Chat</p>
          </div></nuxt-link
        >

        <nuxt-link to="/insights"
          ><div class="side-nav_item">
            <img src="../assets/images/insights.svg" alt="icon" />
            <p>Insights</p>
          </div></nuxt-link
        >
        <nuxt-link to="/config"
          ><div class="side-nav_item">
            <img src="../assets/images/config.svg" alt="icon" />
            <p>API Configuration</p>
          </div></nuxt-link
        >
        <nuxt-link to="/setings"
          ><div class="side-nav_item">
            <img src="../assets/images/settings.svg" alt="icon" />
            <p>Setings</p>
          </div></nuxt-link
        >

        <nuxt-link to="/collapse"
          ><div class="side-nav_item collapse">
            <img src="../assets/images/collapse.svg" alt="icon" />
            <p>Collapse</p>
          </div></nuxt-link
        >
      </nav>
    </div>
    <div class="view">
      <div class="header">
        <div>
          <p>Chat/Direct Messages <span>/XVgQSLEhOFA...</span></p>
        </div>
        <div class="initials">
          <p>AO</p>
          <!-- <div></div> -->
          <img src="../assets/images/path.svg" alt="icon" />
        </div>
      </div>

      <div class="dashboard">
        <div class="dashboard-content">
          <div class="tabs">
            <p>Direct Messages</p>
            <p>Groups</p>
          </div>
          <div class="token">
            <p class="title">User Token</p>
            <p class="code">
              XVgQSLEhOFAXnIKiuXQbtdYY <span class="copy">Copy</span>
            </p>
          </div>

          <div class="meta">
            <p class="meta-data">Meta Data</p>
            <p class="key">Key <span>Value</span></p>
            <p class="name">Name <span>Robin Hood</span></p>
            <p class="url">Profile_url <span>https://bit.ly/123</span></p>
          </div>

          <div class="recentContainer">
            <p class="title">Recent Events</p>

            <div class="recent">
              <div class="vector">
                <p class="line"></p>
              </div>
              <p>Created conversation <br />9th Dec 2020, 12:03</p>
            </div>
            <div class="recent">
              <div class="vector">
                <!-- <p class="line"></p> -->
              </div>
              <p>User Token was created <br />8th Dec 2020, 14:28</p>
            </div>
          </div>
        </div>
        <div class="table-container">
          <table-data />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import tableData from '../components/table-data.vue'
export default {
  components: { tableData },
}
</script>
<style scoped>
* {
  /* background-color: #fff; */
  font-family: 'Inter', sans-serif;
  font-size: 16px;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  color: #5d6970;
  border-style: none;
  border: none;
  font-style: normal;
  font-weight: normal;
}

a {
  text-decoration: none;
}

ul {
  list-style: none;
}

i,
a,
button {
  cursor: pointer;
}

.container {
  background: #f3f7ff !important;
  width: 100%;
  display: flex;
}
.logo {
  margin: 24px 0 31px 20px;
}
.sidebar {
  background: #fff;
  width: 15vw;
  /* height: 100vh; */
  /* margin-right: 52px; */
}
.side-nav_item {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
  height: 60px;
  cursor: pointer;
}
.side-nav_item img {
  padding: 20px 20px 20px 32px;
}

.side-nav_item p {
  width: 100%;
  padding: 21px 16px;
  font-size: 15px;
  margin: 0;
  font-size: 15px;
  line-height: 19px;
  letter-spacing: 0.02em;
  color: #566ba0;
}
.collapse {
  margin: 141px 29px 0 29px;
  border-top: 1px solid #d3d7ea;
}
.view {
  width: 100%;
  background: #f3f7ff;
  /* background: red; */
}
.dashboard {
  display: flex;
}
.header {
  display: flex;
  justify-content: space-between;
  border-bottom: 1px solid #535f89;
  background-color: #f3f7ff;
}
.initials {
  display: flex;
  /* background: yellowgreen; */
  margin-right: 30px;
  /* width: 10%; */
}
.initials p {
  margin-right: 14px;
  /* background: #efefef; */
  border-radius: 20px;
  text-align: center;
  cursor: pointer;
  /* padding: 5px 10px; */
}
.initials img {
  margin-top: 35px;
  cursor: pointer;
}
.header p {
  font-size: 15px;
  line-height: 18px;
  letter-spacing: 0.02em;
  text-transform: capitalize;
  padding: 49px 0 13px 52px;
  color: #566ba0;
  opacity: 0.5;
}

.tabs {
  display: flex;
  margin-left: 52px;
  border-bottom: 1px solid #535f89;
}
.tabs p {
  padding-right: 39px;
  padding-bottom: 29px;
  padding-top: 32px;
}
.tabs p:active {
  font-weight: bold;
  font-size: 17px;
  line-height: 22px;
  letter-spacing: 0.02em;
  border-bottom: 1px solid #d38450;
  color: #d38450;
}

.token {
  background: #ffffff;
  border-radius: 5px;
  width: 28vw;
  height: 21vh;
  margin-left: 52px;
  margin-top: 40px;
}

.token .title,
.recentContainer .title {
  padding: 19px 0 20px 27px;
  color: #566ba0;
  border-bottom: 1px solid #000000;
}
.token .code {
  padding: 28px 0 28px 27px;
  color: #566ba0;
  opacity: 0.9;
}
.token .copy {
  font-size: 12px;
  line-height: 15px;
  color: #ea8d51;
  padding-left: 25px;
}
.meta {
  background: #ffffff;
  border-radius: 5px;
  width: 28vw;
  height: 37vh;
  margin-top: 20px;
  margin-left: 52px;
  margin-bottom: 20px;
}
.meta-data {
  font-size: 14px;
  line-height: 17px;
  color: #566ba0;
  opacity: 0.9;
  padding: 17px 0 18px 27px;
}
.key,
.name,
.url {
  /* opacity: 0.1; */
  border-top: 1px solid #000000;
  padding: 17px 0 25px 27px;
  font-size: 14px;
  line-height: 17px;
  font-weight: normal;
  color: #566ba0;
}
.name span {
  padding-left: 100px;
  color: #566ba0;
  opacity: 0.9;
  font-size: 14px;
  line-height: 15px;
}

.url span {
  padding-left: 74px;
  color: #566ba0;
  opacity: 0.9;
  font-size: 14px;
  line-height: 15px;
}
.key span {
  padding-left: 112px;
  color: #566ba0;
  opacity: 0.5;
  font-size: 14px;
  line-height: 15px;
}
.recentContainer {
  background: #ffffff;
  border-radius: 5px;
  width: 28vw;
  height: 32vh;
  margin-left: 52px;
  margin-top: 40px;
}
.line {
  border-left: 0.5px solid rgba(133, 141, 150, 0.53);
  height: 40px;
  position: absolute;
  margin-left: 4px;
  margin-top: 8px;
}
.vector {
  border-radius: 100%;
  background: #535f89;
  border: 1px solid #ea8d51;
  width: 11px;
  height: 11px;
  margin-left: 25px;
  margin-top: 21px;
}

.recent {
  display: flex;
}
.recent p {
  padding-left: 25px;
  padding-top: 16px;
  font-size: 13px;
  line-height: 16px;
  text-transform: capitalize;

  color: #566ba0;
}
.dashboard-content {
  margin-top: 30px;
}
.table-container {
  /* width: 100%; */
  margin: 150px 22px 50px 22px;
  border-radius: 5px;
}
</style>
