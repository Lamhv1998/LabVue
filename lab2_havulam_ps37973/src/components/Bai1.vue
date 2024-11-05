<template>
  <div class="container md-5 h-25 w-50">
    <h3 class="text-center mt-5">Bảng thành phần dinh dưỡng</h3>
    <table class="table table-bordered table-hover">
      <thead>
        <tr>
          <th
            colspan="4"
            rowspan="2"
            class="align-middle text-center bg-warning"
          >
            Thành phần
          </th>
          <th colspan="2" class="align-middle text-center bg-warning">
            Giá trị
          </th>
        </tr>
        <tr>
          <th class="bg-warning">Khối lượng</th>
          <th class="bg-warning">%DV*</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td colspan="4">Calories</td>
          <td>200 kcal</td>
          <td>20%</td>
        </tr>
        <tr>
          <td colspan="4">Chất béo</td>
          <td>200 kcal</td>
          <td>20%</td>
        </tr>
        <tr>
          <td colspan="4">Chất béo bão hòa</td>
          <td>200 kcal</td>
          <td>20%</td>
        </tr>
        <tr>
          <td colspan="4">Chất đạm</td>
          <td>200 kcal</td>
          <td>20%</td>
        </tr>
        <tr>
          <td colspan="4">Chất sơ</td>
          <td>12g</td>
          <td>-</td>
        </tr>
        <tr>
          <td
            colspan="4"
            rowspan="2"
            style="vertical-align: middle; text-align: left"
          >
            Vitamin
          </td>
          <td>Vitamin C</td>
          <td>25%</td>
        </tr>
        <tr>
          <td>Vitamin D</td>
          <td>10%</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>
<script>
export default {};
</script>
<style>
.table-orange {
  background-color: orange !important;
  color: white !important;
}
table {
  height: 200px;
  width: 300px;
  margin: 20px;
}
</style>
