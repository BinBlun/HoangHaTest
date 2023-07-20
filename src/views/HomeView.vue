<template>
  <div class="home-container">
    <div class="home-first-section">
      <div class="travel-category">
        <p>Du lịch trong nước <i class="fa-solid fa-chevron-right"></i></p>
        <p>Du lịch Trung Quốc <i class="fa-solid fa-chevron-right"></i></p>
        <p>Các tour khác <i class="fa-solid fa-chevron-right"></i></p>
        <p>Cẩm nang <i class="fa-solid fa-chevron-right"></i></p>
        <p>Khuyến mãi <i class="fa-solid fa-chevron-right"></i></p>
      </div>
      <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-indicators">
          <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active"
            aria-current="true" aria-label="Slide 1"></button>
          <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1"
            aria-label="Slide 2"></button>
          <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2"
            aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
          <div class="carousel-item active">
            <img src="../assets/images/Slide.png" class="d-block w-100" alt="...">
            <div class="carousel-caption d-none d-md-block">
              <h5>First slide label</h5>
              <p>Some representative placeholder content for the first slide.</p>
            </div>
          </div>
          <div class="carousel-item">
            <img src="../assets/images/Slide.png" class="d-block w-100" alt="...">
            <div class="carousel-caption d-none d-md-block">
              <h5>Second slide label</h5>
              <p>Some representative placeholder content for the second slide.</p>
            </div>
          </div>
          <div class="carousel-item">
            <img src="../assets/images/Slide.png" class="d-block w-100" alt="...">
            <div class="carousel-caption d-none d-md-block">
              <h5>Third slide label</h5>
              <p>Some representative placeholder content for the third slide.</p>
            </div>
          </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions"
          data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions"
          data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
      <div class="extended-category">
        <div class="extent-item">
          <p>Hà Khẩu</p>
        </div>
        <div class="extent-item">
          <p>DV Visa</p>
        </div>
        <div class="extent-item">
          <p>KS / Dịch vụ</p>
        </div>
      </div>
    </div>
  </div>
  <div class="hot-sale-container">
    <div class="hot-sale-header">
      <img src="../assets/images/fireicon.png" alt="">
      <h2>Hot Sale</h2>
    </div>
    <div class="hot-sale-items">

      <div class="card hot-sale-item" style="width: 22vw;background: none;border: none;">
        <img src="../assets/images/img2.png" class="card-img-top sale-img" alt="...">
        <div class="card-body">
          <h5 class="card-title">Lào Cai - Hà Khẩu - Kiến Thủy 2n1Đ</h5>
          <p>Giá: <span style="font-weight: bold; color: #ff6b00;">3.600.000</span> VNĐ </p>
        </div>
      </div>
      <div class="card hot-sale-item" style="width: 22vw;background: none;border: none;">
        <img src="../assets/images/img2.png" class="card-img-top sale-img" alt="...">
        <div class="card-body">
          <h5 class="card-title">Lào Cai - Hà Khẩu - Kiến Thủy 2n1Đ</h5>
          <p>Giá: <span style="font-weight: bold; color: #ff6b00;">3.600.000</span> VNĐ </p>
        </div>
      </div>
      <div class="card hot-sale-item" style="width: 22vw;background: none;border: none;">
        <img src="../assets/images/img2.png" class="card-img-top sale-img" alt="...">
        <div class="card-body">
          <h5 class="card-title">Lào Cai - Hà Khẩu - Kiến Thủy 2n1Đ</h5>
          <p>Giá: <span style="font-weight: bold; color: #ff6b00;">3.600.000</span> VNĐ </p>
        </div>
      </div>
      <div class="card hot-sale-item" style="width: 22vw;background: none;border: none;">
        <img src="../assets/images/img2.png" class="card-img-top sale-img" alt="...">
        <div class="card-body">
          <h5 class="card-title">Lào Cai - Hà Khẩu - Kiến Thủy 2n1Đ</h5>
          <p>Giá: <span style="font-weight: bold; color: #ff6b00;">3.600.000</span> VNĐ </p>
        </div>
      </div>
    </div>
  </div>
  <div class="domestic-travel-container">
  </div>
</template>

<script>
export default {

}
</script>

<style >
.home-container {
  padding-top: 2rem;
  margin: auto;
  padding: auto;
  width: 85%;
}


.hot-sale-item {
  transition: transform 0.2s ease-in-out;
}

.hot-sale-item:hover {
  transform: scale(1.05);
}

.hot-sale-container {
  margin-top: 6rem !important;
  padding-top: 1rem;
  margin: auto;
  padding: auto;
  width: 100%;
  height: 30rem;
  background-color: #d3ecd7;
  text-overflow: ellipsis;
}

.sale-img {
  border-radius: 1rem;
}

.hot-sale-header {
  display: flex;
  flex-direction: row;
  margin: auto;
  padding: auto;
  width: 12rem
}

.hot-sale-items {
  margin-top: 2rem;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  text-overflow: ellipsis;
}

.home-first-section {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

.travel-category {
  position: relative;
  display: flex;
  width: 15rem;
  padding-left: 1rem;
  padding-top: 1rem;
  padding-bottom: 1rem;
  box-sizing: border-box;
  flex-direction: column;
  justify-content: space-around;
  background-color: #d3ecd7;
  border-radius: 1rem;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
}

.travel-category p {
  font-size: larger;
}

.travel-category i {
  position: absolute;
  right: 15px;
}

.slide {
  width: 50rem;
}

.extended-category {
  width: 15rem;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  max-height: 30rem;

}

.extent-item {
  width: 100%;
  border-radius: 1rem;
  height: 7rem;
  background-color: #d3ecd7;
  text-align: center;
  padding-top: 2.5rem;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;

}

.extent-item p {
  margin: auto;
  padding: auto;
}
</style>