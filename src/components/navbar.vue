<template>
    <div>
        <b-navbar toggleable="lg" type="dark" variant="dark">
            <b-navbar-brand href="#" variant="white">test-vue</b-navbar-brand>

            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav>
                    <b-nav-item to="/">Home</b-nav-item>
                    <b-nav-item href="#">Shop or something</b-nav-item>
                    <b-nav-item to="/reader">Reader</b-nav-item>
                </b-navbar-nav>
             </b-collapse>
        </b-navbar>
</div>
</template>

<style lang="scss" scoped>
#nav a{
    color:white !important;
}
#nav a.router-link-exact-active{
    color: rgb(195, 34, 96);
}
.navbar{
    background-color:rgb(85, 15, 42);
}