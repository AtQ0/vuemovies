<template>
    <div class="navbar">

            <div class="hamburger-container">
                <div class="hamburger-wrapper">
                    <div class="rectA"></div>
                    <div class="rectB"></div>
                    <div class="rectC"></div>
                </div>
            </div>


            <div class="logo-container">
                <div class="logo-wrapper">
                    <h1 class="page-logo"><span class="vue-part-of-logo">Vue</span>Movies</h1>
                </div>
            </div>


            <div class="register-and-login-container">
                <div class="login-btn-container">
                    <div class="login-btn">
                        <p><b>LOGIN</b></p>
                    </div>
                </div>
                <div class="register-btn-container">
                    <div class="register-btn">
                        <p><b>REGISTER</b><b class="the-now-in-register-btn"> NOW</b></p>
                    </div>
                </div>
            </div>




    </div>

</template>

<script setup>

</script>

<style scoped>



.navbar{
    width: 100vw;
    padding-top: 5px;
    padding-bottom: 5px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: fixed;
    top: 0px;
    z-index: 2;
    background-color: rgba(0, 0, 0, 0.5);
    backdrop-filter: blur(2px);
}

.hamburger-container{

    padding: 2px;
    width: 29px;
    margin-left: 20px;
}

.hamburger-wrapper{
    display: flex;
    flex-direction: column;
    gap: 5px;
    padding: 2px;
    cursor: pointer;
}

.rectA, .rectB, .rectC{
    width: 25px;
    height: 2.5px;
    background-color: var(--unselected-white);
    border-radius: 16px;
    transition: background-color 0.25s;

}

.hamburger-wrapper:hover .rectA {
    background-color: var(--selected-white);
}

.hamburger-wrapper:hover .rectB {
    background-color: var(--selected-white);
}

.hamburger-wrapper:hover .rectC {
    background-color: var(--selected-white);
}


.logo-container{
    background-color: red;
    padding: 3px;
    flex-grow: 1;
    display: flex;
    justify-content: flex-start;
    align-items: center;
}

.logo-wrapper{
    background-color: lightblue;
    padding: 2px;
}

.vue-part-of-logo{
    color: var(--vue-green);
}

.register-and-login-container{
    width: 29px;
    margin-right: 20px;
    display: flex;
    justify-content: flex-end;
}

.login-btn-container{
    background-color: orange;
    display: flex;
    justify-content: center;
    align-items: center;
}

.login-btn{
    font-size: var(--mobile-dynamic-letter-size);
    margin-right: 10px;
    background-color: red;
    display: none;
}

.login-btn p{
    cursor: pointer;
}

.register-btn-container{
    display: flex;
    justify-content: center;
    align-items: center;
}


.register-btn{
    background-color: var(--light-gray);
    padding: 5px 15px;
    border-radius: 26px;
    font-size: var(--mobile-dynamic-letter-size);
    cursor: pointer;
    white-space: nowrap;
}

.the-now-in-register-btn{
    display: none;
}





@media screen and (min-width: 460px) {


    .register-and-login-container p{
        font-size: 16px;
    }

}

@media screen and (min-width: 575px) {


    .login-btn{
        display: inline;
    }



    .the-now-in-register-btn{
        display: inline;

    }

}



</style>
