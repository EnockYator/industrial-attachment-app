<template>
    <div id="pageHeader">

        <div class="first-navbar">
            <div class="header-icons">
                <ul>
                    <li><NuxtLink to="icon">&copy;</NuxtLink></li>
                    <li><NuxtLink to="icon">&copy;</NuxtLink></li>
                    <li><NuxtLink to="icon">&copy;</NuxtLink></li>
                    <li><NuxtLink to="icon">&copy;</NuxtLink></li>
                    <li><NuxtLink to="icon">&copy;</NuxtLink></li>
                    
                </ul>
            </div>

            <div class="header-quick-links">
                <ul>
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="about">About Us</NuxtLink></li>
                    <li><NuxtLink to="dashboard">Dashboard</NuxtLink></li>
                    <li><NuxtLink to="">Careers</NuxtLink></li>
                    <li><NuxtLink to="contact">Contact us</NuxtLink></li>
                    
                </ul>
            </div>
        </div>
        
        <div class="second-navbar">
            
            <div class="logo">
                <img class="logo-image" src="/assets/images/kvda-logo-image.png" alt="logo-img">
            </div>

            <div class="nav-bar">
            <ul>
                <!--conditional rendering-->
                <li v-if="!isLoginPage"><NuxtLink to="/login">Login</NuxtLink></li>
                <li v-if="!isSignUp"><NuxtLink to="/signup">Sign up</NuxtLink></li>
            </ul>
            </div>
        </div>

    </div>
</template>

<script setup>
// hide login link on login page header
 




</script>


<style scoped>

*{
    overflow: hidden;
}

#pageHeader{
    height: 150px;
    width: 100vw;
    position: relative;
    top: 0;
    display: flex;
    flex-direction: column;
    flex-wrap: nowrap;
    float: left;
    
}

.first-navbar{
    height: 50px;
    width: 100vw;
    float: left;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    padding: 15px 100px 15px 10px;
    justify-content: space-between;
    background-color: rgba(48, 48, 173, 0.749);
    font-weight: bold
}

.header-icons li,.header-quick-links li{
    padding-left: 50px;
}

.second-navbar{
    height: 100px;
    width: 100vw;
    float: left;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-between;

}

#pageHeader .logo{
    height: 100%;
    width: 300px;
    float: left;
    padding: 10px 0 10px 60px;
}

#pageHeader .logo-image{
    background-position: center;
    background-size: cover; 
}

#pageHeader ul{
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
}

.second-navbar .nav-bar{
    height: 100%;
    float: left;
    padding: 25px;
}

#pageHeader .nav-bar li{
    padding-right: 60px;
}



</style>