<template>
  <div class='container1'>
    <section class='category' >
      <h3>Featured Article - </h3>
      <h3>See All Article > </h3>
    </section>
    <div class="cardSectionCont">

  <section class='cardSection1' v-for="article in articles" :key="article.id" >
    <img :src='article.thumbnail' alt="nail" class='thumbNail' />
    <h6>{{article.title}}</h6>
    <section class='authorContainer'>
      <img :src='article.author.avatar' alt="avatar" class='avatar' />
      <section class='author'>
        <p class='name'>{{article.author.name}}</p>
        <p>{{article.createdAt}}</p>
      </section>
    </section>
  </section>
    </div>
    <section class='moreArticle'>
      <button  type="button" @click="nextPage()" class="btn btn-green" >More Article</button>
    </section>
</div>
</template>

<script>
export default {

  data() {
    return {
      articles: [],
      currentPage: 1
    }
  },
  methods: {
    getArticles() {
      fetch(`https://6328f6acd2c97d8c525f8f80.mockapi.io/api/v1/blogs?p=${this.currentPage}&l=5`)
          .then(response => response.json())
          .then(data =>
              this.articles = data,
          )
    },
    nextPage(){
    if(this.currentPage <= 3) {
      this.currentPage = this.currentPage + 1
      this.getArticles()
    } else {
      this.currentPage = 1
      this.getArticles()
    }
    }
  },
  mounted() {
    this.getArticles(`https://6328f6acd2c97d8c525f8f80.mockapi.io/api/v1/blogs?p=${this.currentPage}&l=5`)
  }
}

</script>

<style>
/*@import '../tailwind.css';*/

.container1 {
  display: flex;
  flex-direction: column;
  background-color: white;
  justify-content: space-evenly;
}

.category {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 50px;
  margin: 0 30px 0 30px;
}

.cardSectionCont {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-content: center;
  width: 400px;
  height: 425px;
  gap: 70px;
  margin: 0px 100px 50px 20px;
  cursor: pointer;
}

.cardSection1 {
  background-color: white;
  box-shadow: 0 40px 40px rgb(226, 226, 226);
  border-radius: 12px;
  cursor: pointer;
}

.thumbNail {
  width: 260px;
  height: 198px;
  margin: 20px 20px 20px 20px;
  align-self: center;
  border-radius: 13px;
}

.cardSection1 h6 {
  margin: 20px 20px 20px 20px;
  text-align: start;
}

.authorContainer {
  display: flex;
  flex-direction: row;
}

.avatar {
  width: 57px;
  height: 57px;
  background-size: cover;
  border-radius: 50%;
  margin: 5px 0 0 20px;
  align-items: center;
}

.author {
  flex-direction: column;
  align-items: flex-start;
  margin: 20px 20px 20px 20px;
  text-align: start;
}

.author p {
  font-size: 10px;
  color: #2B2C34;
  margin: 2px 0 0 5px;
}

.name {
  font-weight: bold;
}

.moreArticle {
  align-self: center;
  margin-bottom: 60px;
  top:20px;
}
/*.btn{}*/
/*.btn-green{}*/
/*.btn {*/
/*  width: 165px;*/
/*  height: 64px;*/
/*  background:#0D2E17;*/
/*  border-radius: 8px;*/
/*  padding: 20px 23px 19px;*/
/*  gap: 10px;*/
/*}*/
</style>