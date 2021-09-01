<template>
  <div class="customer-dashboard__sidebar">
    <nav class="sidebar">
      <div class="logo">
        <img src="/../assets/images/logo.svg" class="logo" alt="logo" />
      </div>
      <nuxt-link to="/"
        ><div class="side-nav_item">
          <img src="/../assets/images/dashboard.svg" alt="icon" />
          <p>Dashboard</p>
        </div></nuxt-link
      >

      <nuxt-link to="/chat"
        ><div class="side-nav_item">
          <img src="/../assets/images/chat.svg" alt="icon" />
          <p>Chat</p>
        </div></nuxt-link
      >

      <nuxt-link to="/insights"
        ><div class="side-nav_item">
          <img src="/../assets/images/insights.svg" alt="icon" />
          <p>Insights</p>
        </div></nuxt-link
      >
      <nuxt-link to="/config"
        ><div class="side-nav_item">
          <img src="/../assets/images/config.svg" alt="icon" />
          <p>API Configuration</p>
        </div></nuxt-link
      >
      <nuxt-link to="/setings"
        ><div class="side-nav_item">
          <img src="/../assets/images/setings.svg" alt="icon" />
          <p>Setings</p>
        </div></nuxt-link
      >

      <nuxt-link to="/collapse"
        ><div class="side-nav_item collapse">
          <img src="/../assets/images/collapse.svg" alt="icon" />
          <p>Collapse</p>
        </div></nuxt-link
      >
    </nav>
  </div>
</template>

<script>
export default {
  name: 'sidenav',
}
</script>

<style scoped>
.customer-dashboard__sidebar {
  background: #fff;
  width: 270px;

  /* position: fixed;
 padding-top: 74px;
  height: 900px; */
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
  color: #6f8a9c;
  width: 100%;
  padding: 21px 16px;
  font-size: 15px;
  margin: 0;
}

a.nuxt-link-exact-active .side-nav_item,
a:hover .side-nav_itemu {
  background-color: rgba(4, 37, 56, 0.076);
}

a.nuxt-link-exact-active p,
a:hover p {
  color: #010025;
  font-weight: 600;
}

a.nuxt-link-exact-active img,
a:hover img {
  background-color: #010025;
  border-radius: 0 20px 20px 0;
}
</style>
