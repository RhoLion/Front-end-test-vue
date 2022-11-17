<template>
  <section class='subscribe'>
    <div>
      <img src="../assets/buzon.png"  type="search" alt="device" />
    </div>
    <h2>Subscribe For The Latest Updates</h2>
    <p>Suscribe to newsletters and never miss the new post every week.</p>
    <section class='search'>
      <input type="search" id="form1" class="form-control" placeholder='Enter your email here...' />
      <button type="button" class="btn btn-green">Subscribe</button>
    </section>
  </section>
</template>

<script>
export default {}
</script>

<style>
.subscribe {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  height: 60%;
}

.subscribe div {
  width: 60px;
  height: 50px;
  padding: 20px;
  background-color: white;
  border-radius: 50%;
  margin-top: 50px;
  margin-right: 50px;
}

.subscribe h2 {
  margin-top: 20px;
  font-size: 36px;
}

.subscribe p {
  color: #C0C0C0;
  font-size: 20px;
  margin-right: 60px;
  margin-top: -10px;
}

.search {
  display: flex;
  flex-direction: row;
}

.search input {
  border: transparent;
  color: #C0C0C0;
  width: 444px;
  height: 67px;
  margin: 10px 10px 50px -55px;
}

.search ::placeholder {
  color: #C0C0C0;
}

.search button {
  width: 145px;
  height: 67px;
  background: #0D2E17;
  border-radius: 8px;
  margin: 10px
}
</style>