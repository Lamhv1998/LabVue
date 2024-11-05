<template>
  <h5>Bài tập ứng dụng model</h5>
  <button @click="handleButtonClick">Tài khoản</button>
  <div class="col-3 card p-3" v-if="isShowTab">
    <ul class="nav nav-tabs">
      <li class="nav-item">
        <a
          class="nav-link-active"
          aria-current="page"
          href="#"
          @click="handleChangeButton('signup')"
          >Đăng Ký</a
        >
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#" @click="handleChangeButton('login')"
          >Đăng Nhập</a
        >
      </li>
    </ul>
  </div>
  <div class="row">
    <!-- Form Đăng Ký Thông Tin -->
    <div class="col-md-6" v-if="tabsActive === 'signup'">
      <div class="card p-4">
        <h5 class="card-title">Form Đăng Ký Thông Tin</h5>
        <form>
          <div class="mb-3">
            <label for="fullname" class="form-label">Họ và Tên</label>
            <input
              type="text"
              class="form-control"
              id="fullname"
              placeholder="Nhập họ và tên"
            />
          </div>
          <div class="mb-3">
            <label for="email" class="form-label">Email</label>
            <input
              type="email"
              class="form-control"
              id="email"
              placeholder="Nhập email"
            />
          </div>
          <div class="mb-3">
            <label for="phone" class="form-label">Số Điện Thoại</label>
            <input
              type="text"
              class="form-control"
              id="phone"
              placeholder="Nhập số điện thoại"
            />
          </div>
          <div class="mb-3">
            <label for="password" class="form-label">Mật Khẩu</label>
            <input
              type="password"
              class="form-control"
              id="password"
              placeholder="Nhập mật khẩu"
            />
          </div>
          <div class="mb-3">
            <label for="confirm-password" class="form-label"
              >Xác Nhận Mật Khẩu</label
            >
            <input
              type="password"
              class="form-control"
              id="confirm-password"
              placeholder="Xác nhận mật khẩu"
            />
          </div>
          <div class="mb-3">
            <label class="form-label">Giới Tính:</label>
            <div>
              <input
                type="radio"
                class="form-check-input"
                name="gender"
                id="male"
                value="Nam"
              />
              <label for="male" class="form-check-label">Nam</label>
              <input
                type="radio"
                class="form-check-input ms-3"
                name="gender"
                id="female"
                value="Nữ"
              />
              <label for="female" class="form-check-label">Nữ</label>
            </div>
          </div>
          <div class="mb-3">
            <label for="language" class="form-label">Ngôn Ngữ</label>
            <select class="form-select" id="language">
              <option selected>Tiếng Việt</option>
              <option>English</option>
              <option>Français</option>
            </select>
          </div>
          <div class="form-check mb-3">
            <input type="checkbox" class="form-check-input" id="terms" />
            <label class="form-check-label" for="terms"
              >Tôi đồng ý với các điều khoản và điều kiện</label
            >
          </div>
          <button type="submit" class="btn btn-primary">Đăng Ký</button>
        </form>
      </div>
    </div>
    <!-- Phần login -->
    <LoginForm v-else-if="tabsActive === 'login'"></LoginForm>
  </div>
</template>
<script setup>
import { ref } from "vue";
import LoginForm from "./LoginForm.vue";
const tabsActive = ref(null);
const isShowTab = ref(false);
const handleButtonClick = () => {
  isShowTab.value = !isShowTab.value;
  if (!isShowTab.value) {
    tabsActive.value = !tabsActive.value;
  }
};
const handleChangeButton = (buttonName) => {
  tabsActive.value = buttonName;
};
</script>
<style></style>
