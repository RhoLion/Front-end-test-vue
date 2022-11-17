<template>
  <footer class='footerContainer'>
    <section class='footerDown'>
      <section class='leftImages'>
        <img src="../assets/Medium.png"  type="search" alt="mediun" />
        <img src="../assets/Vector.png" type="search" alt="vector" />
        <img src="../assets/ig.png" type="search" alt="ig" />
        <img src="../assets/linki.png" type="search" alt="linki" />
      </section>
      <section class='Category'>
        <ul>
          <li><h5 href="Category">CATEGORY</h5></li>
          <li><a href="CSS">CSS</a></li>
          <li><a href="Javascript">Javascript</a></li>
          <li><a href="Taliwind">Taliwind</a></li>
          <li><a href="ReactJS">React JS</a></li>
          <li><a href="MoreCategory">More Category</a></li>
        </ul>
      </section>
      <section class='Category'>
        <ul>
          <li><h5 href="AboutMe">ABOUT ME</h5></li>
          <li><a href="AboutMe">About Me</a></li>
          <li><a href="Projects">Projects</a></li>
          <li><a href="Achievement">Achievement</a></li>
        </ul>
      </section>
      <section class='Category'>
        <ul>
          <li><h5 href="getInTouch">GET IN TOUCH</h5></li>
          <li><a href="number">+62-8XXX-XXX-XX</a></li>
          <li><a href="email">demo@gmail.com</a></li>
        </ul>
      </section>
      <section class='Category'>
        <ul>
          <li><h5 href="FollowUs">FOLLOW US</h5></li>
          <li><a href="Medium">Medium</a></li>
          <li><a href="Instagram">Instagram</a></li>
          <li><a href="Twitter">Twitter</a></li>
          <li><a href="Facebook">Facebook</a></li>
        </ul>
      </section>
    </section>
    <section class='koltin'>
      <p>© 2022 Koltin</p>
      <p>Made with <span><img src="../assets/love.png" alt='heart' /></span> México</p>
    </section>
  </footer>
</template>

<script>
export default {}
</script>

<style>
.footerContainer {
  display: flex;
  flex-direction: column;
}

.footerDown {
  display: flex;
  justify-content: space-evenly;
  background-color: #E4E5E9;
  border-bottom: 1px solid #c8c7c7
}

.leftImages{
  display:flex;
  flex-direction: row;
}

.leftImages img {
  width: 25px;
  height: 20px;
  margin: 55px 20px;
}

.Category ul {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 30px 0 20px 0;
  text-align: start;
}

.Category li {
  list-style-type: none;
  padding: 5px;
  font-size: medium;
  color: black;
}

.Category a {
  text-decoration: none;
  color: #2B2C34;
}

.koltin {
  display: flex;
  justify-content: space-around;
  font-size: small;
  margin-top: 20px;
}

.koltin img{
  width: 13px;
  height:12px;
}
</style>