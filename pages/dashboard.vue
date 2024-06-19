<template>
    <div id="dashboard">

        <!---------left bar-------->

        <div class="left-bar flex-item">
            <div class="account-preview left-bar-flex-item">
                <div class="profile-picture"></div>
                <div class="username">
                    <ul>
                        <li><h3 class="name">User name</h3></li>
                        <li><h4>role</h4></li>
                        <li><button class="logout-btn">[- Logout</button></li>
                    </ul>                   
                     
                </div>
            </div>
            <div class="profile-manipulation left-bar-flex-item">
                <div class="heading pm-flex-item">
                    <h3>[] Profile</h3>
                </div>
                <div class="update-profile-link pm-flex-item">
                    <div class="link-name">
                        <NuxtLink to="profile-update">Update profile</NuxtLink>
                    </div>
                    <div class="icon">[]</div>
                    
                </div>
                <div class="application-status pm-flex-item">
                    <div class="link-name">
                        <NuxtLink to="application-status">My application</NuxtLink>
                    </div>
                    <div class="icon">[]</div>
                </div>

            </div>
            <div class="language left-bar-flex-item">
                <div class="language-icon">[]</div>
                <div class="language-name">English (English)</div>
            </div>
            <div class="support-centre left-bar-flex-item">
                <div class="contact-support">
                    <div class="contact-support-icon">[]</div>
                    <div class="contact-support-link">
                        <NuxtLink to="contact-support">Contact support</NuxtLink></div>
                </div>
                <div class="feedback">
                    <NuxtLink to="feedback">Feedback</NuxtLink>
                </div>
                <div class="bottom-logout-btn">[- Logout</div>
            </div>
        </div>


        <!----------main bar----------->

        <div class="main-bar flex-item">
            <div class="top">
                <div class="welcome-container">
                    <h1 class="welcome-item">Welcome!</h1>
                    <p class="welcome-item">Good to see {First Name}.</p>
                    <p class="welcome-item">Explore your account.</p>
                </div>
                <div class="icons-container"></div>
            </div>
            <div class="bottom"></div>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

#dashboard{
    height:100vh !important;
    width: 100vw !important;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    overflow: hidden;
}

/*******left bar***** */

.left-bar{
    width: 20% !important;
    height: 100vh !important;
    display: flex;
    flex-direction: column;
    border-right: 1px solid rgba(0, 0, 0, 0.279) !important;
    box-shadow: 2px 2px rgba(0, 0, 0, 0.113);
}

.left-bar-flex-item{
    border-bottom: 1px solid rgba(0, 0, 0, 0.281);
    margin-bottom: 10px;
    padding: 10px 10px;

}

.account-preview{
    height: 30% !important;
    width: 100% !important;
    display: flex;
    flex-direction: column;
    align-content: center;
    background-color: rgba(128, 128, 128, 0.363);
}


.profile-picture{
    width: 100px;
    height: 150px;
    border-radius: 100%;
    margin: 10px auto 0 auto;
    background-color: rgba(128, 128, 128, 0.767);
}

.username{
    width: 80%;
    height: 50%;
    align-content: center;
    margin: auto;
}

.username .name{
    font-size: 20px;
    color: blue;

}

.username li{
    list-style: none !important;
    text-align: center;
    margin: 5px 0;
}

.logout-btn{
    width: fit-content;
    cursor: pointer;
    background-color: rgb(220, 245, 244);
    border: 2px solid blue;
    padding: 2px 8px;
    border-radius: 5px;
    margin-bottom: 10px;
}

.profile-manipulation{
    height: 30% !important;
    width: 100% !important;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 20px 10px;
    background-color: grey;
}

.profile-manipulation .pm-flex-item{
    width: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-between;
    padding: 10px 10px;
    margin: 2px auto;
    background-color: white;
    border-radius: 10px;
}

.profile-manipulation .heading h3{
    text-align: center;
    font-size: 18px;
    margin: auto;
}

.profile-manipulation div .link-name{
    width: 80% !important;
    height: 100%;
    font-size: 18px;
}

.profile-manipulation div .icon{
    width: 20% !important;
    height: 100%;
}

.language{
    height: 10%;
    border-radius: 10px;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-between;
    background-color: grey;
}

.language-icon{
    width: 20% !important;
    height: 100%;
    font-size: 18px;
    align-content: center;
    padding-left: 5px;
    background-color: aquamarine;
    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
}

.language-name{
    width: 80% !important;
    height: 100%;
    align-content: center;
    padding-left: 5px;
    background-color: aquamarine;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
}

.support-centre{
    height: 30% !important;
    width: 100% !important;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 20px 5px;
    background-color: grey;
}

.contact-support{
    width: 80%;
    height: 30%;
    margin: 0 auto;
    border-radius: 10px;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-between;
    background-color: white;
}

.contact-support-icon{
    width: 20% !important;
    height: 100%;
    align-content: center;
    padding-left: 5px;
    background-color: aquamarine;
    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
}

.contact-support-link{
    width: 80% !important;
    height: 100%;
    font-size: 18px;
    align-content: center;
    padding-left: 5px;
    background-color: aquamarine;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
}

.feedback{
    width: 80%;
    height: 30%;
    margin: 0 auto;
    align-content: center;
    padding-left: 10px;
    border-radius: 10px;
    background-color: aquamarine;
}

.bottom-logout-btn{
    width: fit-content;
    cursor: pointer;
    background-color: rgb(220, 245, 244);
    border: 2px solid blue;
    padding: 2px 8px;
    border-radius: 5px;
    margin: 20px auto 0;
    
}


/**********main bar**********/

.main-bar{
    width: 80% !important;
    height: 100vw !important;
    display: flex;
    flex-direction: column;
    flex-wrap: nowrap;
}

.main-bar .top{
    width: 100%;
    height: 150px;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    box-shadow: 2px 2px rgba(93, 96, 96, 0.433);
}

.welcome-container{
    width: 100%;
    height: 100%;
    align-content: center;
    padding-left: 50px ;
}

.icons-container{
    width: 100%;
    height: 100%;
    background-color: rgba(144, 221, 221, 0.322);
}

.welcome-item{
    margin: 5px auto;
}

.welcome-container h1{
    margin-left: 10px;
    font-size: 25px;
    color: blue;
    margin-bottom: 10px;
}

.welcome-container p{
    font-size: 18px;
}






</style>