<template>
<div>
    <div id="popup" style="display: none;"></div>
    <button type="button" id="adjustview" onclick="change()"></button>
    <div class="container-fluid logos bg-primary">
         <a href="/">
             <img class="mx-auto d-block img-fluid" style="padding-top: 1vh;" src="/images/logo3.png">
        </a>
    <nav class="navbar navbar-expand-lg justify-content-between bg-transparent navbar-light">
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto">
                <li class="nav-item">
                     <a class="nav-link" href="/">Główna</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="/manga">Manga</a>
                </li>
                <li class="nav-item dropdown">
                    <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Wiki</a>
                    <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                       <a class="dropdown-item" href="/DICtionary">Słowniczek</a>
                       <a class="dropdown-item" href="/faq">FAQ o HentaiHaven.pl</a>
                       <a class="dropdown-item" href="/blog">Hentajowy Blog</a>
                    </div>
                </li>
            </ul>
                <form class="form-inline">
                    <input class="form-control mr-sm-2" type="search" placeholder="tag, tytuł, autor" id="tagse">
                    <button class="btn btn-dark my-2 my-sm-0" type="button" onclick="search()">Wyszukaj</button>
                </form>
        </div>
    </nav>
    </div>

    <div class="featured">
      ds
    </div>
    <div class="jumbotron row entryinfobox" id="eib">
        <div class="col-md-4 multi-collapse collapse show">
             <img src='/manga/3/001.jpg' class="mx-auto d-block">
        </div>   
        <div class="align-self-center entryinfoboxtags col-md-8 multi-collapse collapse show">
            <h4>Seria: <a href='/search/'></a></h4>
	        <h4>Postacie: <a href='/search/ss'>ss</a></h4>
            <h4>Tagi: <a href='/search/df'>df</a> </h4>
            <h4>Autor: ew</h4>
            
            <h4>Tłumaczenie: HentaiHaven.pl</h4>
        </div>
        <div class="col-md-12">
            <button class="btn btn-dark mx-auto d-block" type="button" data-toggle="collapse" data-target=".multi-collapse" aria-expanded="true" aria-controls="collapseExample" style="font-family: 'Rubik', sans-serif;">
                zwiń/rozwiń informacje
            </button>
        </div>
    </div>
    <div class="container-fluid readercontainer">
        <button type ="button" class="btnst" onclick="hentieprev()" id="btn_prev" disabled>&#8249;</button>
            <img id = "page"  onclick="hentienext()" src="" class="reader"/>
        <button type="button" class="btnst" onclick="hentienext()" id="btn_next">&#8250;</button>
    </div>
    <div class="pgcounter">
        <button type ="button" class="btnsts" onclick="hentieprev()" id="btn_prevs" disabled>&#8249;</button>
       <h5 id="pgcounter">ds</h5>
        <button type="button" class="btnsts" onclick="hentienext()" id="btn_nexts">&#8250;</button>
    </div>
    <div class="jumbotron" style="background-color:rgba(195, 34, 96, 0.25); color:white; font-family: 'Rubik', sans-serif;" id="infobox">
        <h4>Autor na pewno doceni, jeśli okażesz mu trochę miłości</h4>
        <h6>Autor: ew</h6>
        <a target="_blank" href=sd style="color: rgb(34, 157, 195);"><h6>Strona autora</h6></a>
        <a target="_blank" href=sd style="color: rgb(34, 157, 195);"><h6>Wsparcie dla autora</h6></a>
    </div>

    <div class="feetarentsexy">
        <a href="/contact" class="text-dark"><u>HentaiHaven.pl team</u></a> <br>
        Please don't hack us
        <p><small>Wszystkie postacie przedstawione na tej stronie są pełnoletnie.</small></p>
    </div>
</div>

</template>