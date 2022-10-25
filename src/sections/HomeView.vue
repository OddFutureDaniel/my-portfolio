<template>
    <v-container class="homeContainer">
        <nav class="nav__left">
            <div class="nav__left__items">
                <div class="nav__left__item">{{cv}}</div>
                <div class="nav__left__item">{{linkedIn}}</div>
                <div class="nav__left__item">{{github}}</div>
                <div class="divider">
                    <v-divider class="test" vertical="true" role="presentation"></v-divider>
                </div>
            </div>
            <div class="nav__right__items">
                <div class="nav__right__item">{{text}}</div>
            </div>

        </nav>
        <div class="main__section">
            <div class="section__left">
                <p>{{name}}</p>
                <v-divider width="80%" style="border-color:black"></v-divider>
                <p>{{description}}</p>
            </div>
            <div class="section__right">
                <div class="nav__right">
                    <div class="nav__links">
                        <a class="nav__link" href="">WORK</a>
                    </div>
                    <div class="nav__links">
                        <a class="nav__link" href="">ABOUT</a>
                    </div>
                    <div class="nav__links">
                        <a class="nav__link" href="">CONTACT</a>
                    </div>

                </div>

            </div>
        </div>

    </v-container>
</template>

<script>
export default {
    name: 'HomeView',

    data: () => ({
        title: "Hey bro",
        cv: "CV",
        linkedIn: "LI",
        github: "GH",
        text: "Designed & created by Daniel Rogerson",
        name: "Daniel Rogerson",
        description: "Frontend Web Developer & Designer",
    })
}
//rgb(82, 183, 189) tiffany blue - matches fuschia
</script>
<style>
.homeContainer {
    min-height: 100vh;
    min-width: 100vw;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: row;
    background-color: rgb(234, 219, 208);
}


.nav__left {
    position: fixed;
    width: 6vw;
    display: flex;
    height: 100vh;
    flex-direction: column;
    margin-top: 5%;
    justify-content: space-between;
    min-width: 65px;
}



.nav__left__item {
    margin-bottom: 40px;
    padding-right: 15px;
    padding-left: 20px;

    transform: rotate(-90deg);
}

.test {
    border-color: black;
    height: 113px;
    max-width: 100px;
    border-width: 0.5px;
    /* transform: rotate(-90deg); */
    /* margin-top: 1px; */
    margin-left: 32px;
}

.divider {
    width: 100%;
}

.nav__right__item {
    margin-top: 180px;
    margin-left: -107px;
    width: max-content;
    transform: rotate(-90deg);
}

.nav__right__items {
    width: 100%;
    height: 100%;
}

.main__section {
    display: flex;
    min-width: 94vw;
    margin-left: 6vw;
}

.section__left {
    width: 35%;
    padding-top: 63vh;
    padding-left: 10%;
}

.section__right {
    width: 65%;
    height: 100vh;
}

.nav__right {
    padding-top: 13%;
    padding-bottom: 13%;
    display: flex;
    flex-direction: column;
    height: 100vh;
    justify-content: space-between;
}

.nav__links {
    display: flex;
    position: relative;
    height: 33.3%;
}

.nav__link {
    font-family: "Extatica";
    font-size: 12em;
    text-decoration: none;
    color:  rgb(63, 33, 1);
    line-height: 0.95em;
}

.nav__link:hover{
    color: rgb(82, 183, 189);
}

@font-face {
    font-family: "Extatica";
    src: local("Extatica"), url("../fonts/Extatica/Extatica-Medium.otf");
}

@media screen {
    
}
</style>