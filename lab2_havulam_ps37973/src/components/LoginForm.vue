<template>
  <div class="col-md-4">
    <div class="card p-4">
      <h5 class="card-title">Form Đăng Nhập</h5>
      <form>
        <div class="mb-3">
          <label for="login-email" class="form-label">Email</label>
          <input
            type="email"
            class="form-control"
            id="login-email"
            placeholder="Nhập email"
          />
        </div>
        <div class="mb-3">
          <label for="login-password" class="form-label">Mật Khẩu</label>
          <input
            type="password"
            class="form-control"
            id="login-password"
            placeholder="Nhập mật khẩu"
          />
        </div>
        <button type="submit" class="btn btn-primary">Đăng Nhập</button>
      </form>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style></style>
