<script>
import { RouterLink, RouterView } from 'vue-router'
import { toast } from 'vue3-toastify';
import 'vue3-toastify/dist/index.css';
import { onMounted } from 'vue';
import PageFooter from './components/PageFooter.vue'
export default {
  components: { PageFooter },
  name: "App",
  setup() {
    const notify = () => {
      toast.warn("Trang web đang trong quá trình xây dựng, còn nhiều thiết sót mong bạn thông cảm", {
        autoClose: 60000,
        theme: "dark",
        position: toast.POSITION.BOTTOM_RIGHT,
      });
    }
    function scrollToTop() {
      window.scrollTo(0, this.top);

    }
    onMounted(() => {
      notify()
    })
    return { scrollToTop };
  }
};

</script>

<template>
  <div class="header-container">
    <div class="banner-text">
      <p class="company-name">HOÀNG HÀ</p>
      <p class="subtext-1">travel and tourism</p>
    </div>
    <img src="./assets/stamp.png" alt="" class="stamp">
    <img src="./assets/header1.png" alt="" class="banner">
    <nav class="navbar navbar-expand-lg custom-bg">
      <div class="container-fluid">
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-5 mb-lg-0">
            <!-- <li class="nav-item">
              <RouterLink class="nav-link active" to="/" aria-current="page" href="#">Trang Chủ</RouterLink>
            </li> -->
            <div class="vl"></div>

            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                DANH MỤC
              </a>

              <ul class="dropdown-menu">
                <li>
                  <RouterLink class="nav-link active" to="/" aria-current="page" href="#">Trang chủ</RouterLink>
                </li>
                <li>
                  <hr class="dropdown-divider">
                </li>
                <li>
                  <RouterLink class="nav-link active" to="/foreigntravel" aria-current="page" href="#">Du lịch trong nước
                  </RouterLink>
                </li>
                <li>
                  <RouterLink class="nav-link active" to="/foreigntravel" aria-current="page" href="#">Du lịch quốc tế
                  </RouterLink>
                </li>
                <li>
                  <RouterLink class="nav-link active" to="/foreigntravel" aria-current="page" href="#">Loại tour
                  </RouterLink>
                </li>
                <li>
                  <RouterLink class="nav-link active" to="/foreigntravel" aria-current="page" href="#">Dịch vụ du lịch
                  </RouterLink>
                </li>
                <li>
                  <RouterLink class="nav-link active" to="/foreigntravel" aria-current="page" href="#">Cẩm nang
                  </RouterLink>
                </li>
              </ul>
            </li>
            <div class="vl"></div>
            <!-- <li class="nav-item">
              <RouterLink class="nav-link active" to="/register" aria-current="page" href="#">Đăng ký</RouterLink>
            </li> -->
            <form class="d-flex search-container">
              <button class="btn btn-outline-success" type="submit"><i class="fas fa-search"></i></button>
              <input class="form-control me-2 search-box" type="search" placeholder="Search" aria-label="Search">
            </form>
            <li class="nav-item hotline">
              <RouterLink class="nav-link active" to="/" aria-current="page" href="#">HOTLINE: <span
                  style="color: rgb(255, 208, 0);">0123454952</span>
                <img src="./assets/call-center.png" alt="" class="call-icon">
              </RouterLink>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
  <div class="content-container">
    <RouterView />
  </div>
  <div class="scroll-top">
    <button type="button" class="btn btn-success scroll-button" @click="scrollToTop"><i
        class="fa-solid fa-arrow-up"></i></button>
  </div>
  <div class="spacer" style="height: 8rem;"></div>
  <PageFooter></PageFooter>
</template>

<style scoped>
.header-container {
  position: relative;
}

.banner-text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-47%, -70%);
  display: flex;
  flex-direction: row;
  align-items: flex-end;
}

.company-name {
  color: #045B48;
  font-size: 5em;
  font-weight: bold;
}

.vl {
  width: 1rem;
  border-left: 1px solid #045B48;
}

.subtext-1 {
  color: #045B48;

  font-size: larger;
  padding-left: 1rem;
  padding-bottom: 1.3rem;
}

.stamp {
  position: absolute;
  top: 1rem;
  left: 1rem;
}

.call-icon {
  width: 2.2rem;
  padding-bottom: 0.2rem;
}

nav {
  padding: 0.35rem;
  padding-left: 3rem;
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 100%;
  z-index: 9999;
  position: absolute;
  bottom: 0;
}

.custom-bg {
  background-color: rgba(255, 255, 255, 0.247);
  ;
}

.banner {
  width: 100%;
  display: block;
  margin-left: auto;
  margin-right: auto;
}

.nav-link {
  color: #045B48 !important;
  margin-left: 0.2rem;
  margin-right: 0.2rem;
  font-size: larger;
  font-weight: 500;
  transition: border-bottom 0.2s linear color 0.2s linear;
  border-bottom: 1px solid transparent;
}

.dropdown-menu {
  /* margin-top: 1rem; */
  background-color: #dbebe1;
}

.nav-link:hover {
  border-bottom: 1px solid #ffffff;
  color: white;
}


.scroll-top {
  position: fixed;
  bottom: 2rem;
  right: 2rem;
}

.scroll-button {
  height: 3rem;
  width: 3rem;
  border-radius: 20rem;
  transition: transform 0.2s ease-in-out;
  z-index: 9999 !important;
}

.scroll-button:hover {
  transform: scale(1.1);
}

.search-box {
  background: none;
  margin-left: 1rem;
}

.search-container {
  margin-left: 2rem;
}

.hotline {
  position: absolute;
  right: 5rem;
}

@media screen and (max-width: 1214px) {
  .company-name {
    font-size: 3em;
  }
}

@media screen and (max-width: 860px) {
  .company-name {
    font-size: 2em;
  }
}
</style>
