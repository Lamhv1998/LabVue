<template>
  <nav class="navbar navbar-expand-sm navbar-dark">
    <div class="container m-auto px-5">
      <a class="navbar-brand" href="">
        <img src="../assets/images/logo-energy-pilates.png" />
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#collapsibleNavbar"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="collapsibleNavbar">
        <ul class="navbar-nav me-auto">
          <li class="nav-item">
            <a class="nav-link" href="#"
              ><i class="fa-solid fa-list"></i>Bài Viết</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <i class="fa-solid fa-video"></i>Video</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="App.vue"
              ><i class="fa-solid fa-circle-info"></i>Giới thiệu</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="App.vue"
              ><i class="fa-solid fa-calendar-days"></i>Sự kiện</a
            >
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
              style="color: black"
            >
              <i class="fa-solid fa-user"></i>Tài khoản
            </a>
            <ul class="dropdown-menu">
              <li><a href="#" class="dropdown-item">Đăng nhập</a></li>
              <li><a href="#" class="dropdown-item">Quên mật khẩu</a></li>
              <li><a href="#" class="dropdown-item">Đăng kí thành viên</a></li>
            </ul>
          </li>
        </ul>
        <ul class="navbar-nav d-flex">
          <li class="nav-item me-3">
            <a href="#" style="color: black">Tiếng Việt</a>
          </li>
          <li class="nav-item">
            <a href="#" style="color: black">Tiếng Anh</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
<script></script>
<style>
html,
body {
  height: 100%; /* Chiều cao 100% cho body */
  margin: 0; /* Bỏ margin mặc định của trình duyệt */
}
img {
  width: 150px;
}
a {
  padding-right: 5px;
  color: black !important;
  i {
    padding-inline: 5px;
  } 
}
</style>
