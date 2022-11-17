<template>
  <section class='md:flex justify-between ml-20 mr-20 mb-8 mt-8 font-bold font-primaryFont'  >
    <h3>Browse The Category -</h3>
    <h3>See All Category > </h3>
  </section>
  <div class="md:flex justify-around mt-2">
    <section class='cardSection' >
      <img src="../assets/CSS.png" class="w-10 mt-24" alt="css" />
      <h5>CSS</h5>
    </section>
    <section class='cardSection' >
      <h2>JS</h2>
      <h5>Javascript</h5>
    </section>
    <section class='cardSectionBlack' >
      <img src="../assets/tailwind.png" alt="tailwind" />
      <h5>Tailwind</h5>
    </section>
    <section class='cardSection' >
      <img src="../assets/vue.png" alt="vue" />
      <h5>Vue JS</h5>
    </section>
    <section class=cardSection >
      <img src="../assets/react.png" alt="react" />
      <h5>React JS</h5>
    </section>
  </div>
</template>

<script>
export default {}
</script>

<style>
body {
  background-color: #EFF0F3;
}

.container {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
}

.cardSection {
  display: flex;
  flex-direction: column;
  width: 220px;
  height: 280px;
  background-color: white;
  border-radius: 8px;
  margin: 10px 0 100px;
}

.cardSection img {
  width: 35px;
  height: 35px;
  margin: 100px 50px 0 50px;
}

.cardSection h5 {
  margin: 30px 50px;
}

.cardSection h2 {
  margin: 100px 50px 0 50px;
}

.cardSectionBlack {
  display: flex;
  flex-direction: column;
  width: 220px;
  height: 280px;
  border-radius: 8px;
  background-color: #0D2E17;
  color: white;
  margin: 10px;
}

.cardSectionBlack img {
  width: 47px;
  height: 50px;
  margin: 90px 50px 0 50px;
  border-radius: 8px;

}

.cardSectionBlack h5 {
  margin: 30px 50px;
}

.category {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  margin: 50px 200px 50px 200px;
}
</style>