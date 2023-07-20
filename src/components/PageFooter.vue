<template>
    <div class="footer-container">
        <div class="footer-head">
            <div class="footer-head-item">
                <img src="../assets/images/ftimg1.png" class="footer-head-icon" alt="">
                <div class="footer-head-text">
                    <p><span style="color: #ff6b00; font-weight: bold;">TƯ VẤN 24/7</span></p>
                    <p><span style="color: white;">Tổng đài tư vấn 349349</span></p>
                    <p><span style="color: white;">Hỗ trợ 24/7</span></p>
                </div>
            </div>
            <div class="footer-head-item">
                <img src="../assets/images/ftimg2.png" class="footer-head-icon" alt="">
                <div class="footer-head-text">
                    <p><span style="color: #ff6b00; font-weight: bold;">BẢO HIỂM DỊCH VỤ</span></p>
                    <p><span style="color: white;">Cam kết hoàn tiền nếu Dịch vụ</span></p>
                    <p><span style="color: white;">không đúng</span></p>
                </div>
            </div>
            <div class="footer-head-item">
                <img src="../assets/images/ftimg3.png" class="footer-head-icon" alt="">
                <div class="footer-head-text">
                    <p><span style="color: #ff6b00; font-weight: bold;">CHẤT LƯỢNG HÀNG ĐẦU</span></p>
                    <p><span style="color: white;">Không cạnh tranh về giá, chỉ</span></p>
                    <p><span style="color: white;">tập trung vào chất lượng</span></p>
                </div>
            </div>
            <div class="footer-head-item">
                <img src="../assets/images/ftimg4.png" class="footer-head-icon" alt="">
                <div class="footer-head-text">
                    <p><span style="color: #ff6b00; font-weight: bold;">NIỀM TIN PHÁT TRIỂN</span></p>
                    <p><span style="color: white;">Nỗ lực phát tiển để trở thành Công</span></p>
                    <p><span style="color: white;">ty lữ hành hàng đầu tại Lào Cai</span></p>
                </div>
            </div>

        </div>
        <div class="footer-main-content">
            <div class="footer-section footer-section-1">
                <div class="section-top-bar"></div>
                <h3>CÔNG TY TNHH MTV DU LỊCH QUỐC TẾ HOÀNG HÀ</h3>
            </div>
            <div class="footer-section">
                <div class="section-top-bar"></div>
                <h3>Đăng ký tư vấn</h3>
            </div>
            <div class="footer-section footer-section-2">
                <div class="section-top-bar"></div>
                <h2>Đăng ký tư vấn</h2>
                <div class="footer-form">
                    <input class="form-control footer-input" type="text" placeholder="Họ tên"
                        aria-label="default input example">
                    <input class="form-control footer-input" type="text" placeholder="Số điện thoại"
                        aria-label="default input example">
                    <input class="form-control footer-input" type="text" placeholder="Email"
                        aria-label="default input example">
                    <textarea class="form-control footer-text-area" placeholder="Ghi chú" id="floatingTextarea"></textarea>
                </div>
                <button type="button" class="btn btn-success footer-form-button">Đăng ký</button>

            </div>
        </div>
        <img src="../assets/images/footer-img.png" class="footer-img" alt="">
        <div class="footer-main-content">
        </div>
    </div>
</template>

<script>
export default {
    name: 'footer',
}
</script>
<style >
.footer-container {
    position: relative;
    width: 100%;
}

.footer-img {
    width: 100%;
}

.footer-head {
    display: flex;
    padding-top: 0.8rem;
    padding-bottom: 0.8rem;
    flex-direction: row;
    height: 6rem;
    background-color: #045B48;
    justify-content: space-around;
    box-shadow: rgba(0, 0, 0, 0.644) 0px 6px 8px;

}

.footer-head-item {
    display: flex;
    gap: 1rem;
    flex-direction: row;
}

.footer-head-text {
    display: flex;
    flex-direction: column;
}

.footer-head-text p {
    margin: 0;
    padding: 0;
}

.footer-main-content {
    position: absolute;
    top: 9rem;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding-left: 2rem;
    padding-right: 5rem;
    width: 100%;
}

.section-top-bar {
    border-top: 3px solid #045b48;
    height: 1rem;
}

.footer-section-1 {
    width: 25rem;
    color: #045b48;
}

.footer-section-2 {
    color: #045b48;
    width: 25rem;
    position: relative;

}

.footer-form {
    display: flex;
    flex-direction: column;
    gap: 2rem;
}

.footer-input {
    height: 3rem;
    border-radius: 0.7rem;
    background-color: #dbebe1;
    border: 1px solid #a1ffc5;
}

.footer-form-button {
    margin-top: 2rem;
    position: absolute;
    right: 0;
}

.footer-note-input {
    height: 8rem;
}

.footer-text-area {
    border-radius: 0.7rem;
    height: 8rem;
    background-color: #dbebe1;
    border: 1px solid #a1ffc5;
}

textarea {
    resize: none;
}
</style>