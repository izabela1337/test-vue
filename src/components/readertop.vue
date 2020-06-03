<template>
  <div class="container">
    <div class="featured">
      Pokusa Anioła
    </div>
    <div class="jumbotron row entryinfobox" id="eib">
      <div class="col-md-4 multi-collapse collapse show">
        <img src="/manga/3/001.jpg" class="mx-auto d-block" />
      </div>
      <div
        class="align-self-center entryinfoboxtags col-md-8 multi-collapse collapse show"
      >
        <h4>Seria: <a href="/search/Hugtto Precure">Hugtto Precure</a></h4>
        <h4>
          Postacie:
          <a href="/search/Yakushiji Saaya (Cure Ange)"
            >Yakushiji Saaya (Cure Ange)</a
          >
        </h4>
        <h4>
          Tagi: <a href="/search/yuri">yuri</a>
          <a href="/search/nauczycielka">nauczycielka</a>
          <a href="/search/palcówka">palcówka</a>
          <a href="/search/różnica wieku">różnica wieku</a>
          <a href="/search/okulary">okulary</a>
          <a href="/search/miłość">miłość</a>
        </h4>
        <h4>Autor: Negom</h4>

        <h4>Tłumaczenie: HentaiHaven.pl</h4>
      </div>
      <div class="col-md-12">
        <button
          class="btn btn-dark mx-auto d-block"
          type="button"
          data-toggle="collapse"
          data-target=".multi-collapse"
          aria-expanded="true"
          aria-controls="collapseExample"
          style="font-family: 'Rubik', sans-serif;"
        >
          zwiń/rozwiń informacje
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.featured {
  font-family: "Rubik", sans-serif;
  font-size: 20pt;
  color: white;
  padding: 10px;
}
.entryinfobox {
  background-color: rgba(195, 34, 96, 0.25);
  background-image: url("/images/sitebg.png");
  background-size: cover;
  color: white;
  margin: 2vh;
  padding: 10px;
}
.entryinfobox img {
  display: flex;
  height: 400px;
  width: auto;
  max-height: 35vh;
  margin-bottom: 10px;
  margin-top: 10px;
}
.entryinfoboxtags h4 {
  padding: 6px 0 6px 0;
  font-family: "Josefin Sans", sans-serif;
  line-height: 1.5;
}
.entryinfoboxtags a {
  color: black;
  background-color: rgb(195, 34, 96);
  border-radius: 5px;
  padding: 4px;
  margin: 0 10px 0 10px;
  white-space: nowrap;
}
</style>
