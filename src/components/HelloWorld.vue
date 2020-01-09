<template>
  <div class="col-5">
    <div class="col-12">
      <h5 class="text-center m-top">Pendaftaran Online</h5>
      <div>
        <div>Nama</div>
        <input type="text" placeholder="Nama" class="form-control" />
        <div>Tanggal Lahir</div>
        <input type="date" placeholder="Tanggal Lahir" class="form-control" />
        <div>Jenis kelamin</div>
        <b-form-input list="my-list-id"></b-form-input>
        <datalist id="my-list-id">
          <option v-for="kelamin in kelamins" :key="kelamin">{{kelamin}}</option>
        </datalist>
        <div>Alamat</div>
        <textarea placeholder="Alamat" class="form-control"></textarea>
        <div>Daftar Riwayat Hidup</div>
        <textarea placeholder="Riwayat Hidup" class="form-control"></textarea>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  data() {
    return {
      kelamins: ["Pria", "Wanita"]
    };
  }
};
</script>

<style>
.m-top {
  margin-top: 20px;
}
</style>
