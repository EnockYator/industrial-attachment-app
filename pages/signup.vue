<template>
    <PageHeader />
    <div id="signupPage">
        <div class="signup-container">
            <div class="signup-heading">
                <h3>Sign Up</h3>
            </div>

            <div class="signup-form">
                <form>
                    <label for="firstName">First Name:</label>
                    <input type="text" name="firstName" id="firstName" placeholder="First Name" required>

                    <label for="secondName">Second Name:</label>
                    <input type="text" name="secondName" id="secondName" placeholder="Second Name" required>

                    <label for="email">Email:</label>
                    <input type="email" name="email" id="email" placeholder="Email address" required>

                    <label for="password">Password:</label>
                    <input type="password" name="password" id="password" placeholder="Password" required>

                    <label for="confirmedPassword">Password:</label>
                    <input type="password" name="confirmedPassword" id="confirmedPassword" placeholder="Confirm Password" required>

                    <button type="submit" class="signup-btn">Signup</button>

                    <p>
                        Already have an account? 
                        <NuxtLink to="signup" class="signup-alternative">
                            Login<span> here</span>
                        </NuxtLink>
                    </p>
                </form>
            </div>
        </div>
    </div>

    <PageFooter />
</template>

<script setup>

</script>

<style scoped>

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

#signupPage{
    height: fit-content;
    width: 100vw;
    float: left;
    margin: 20px auto;

}

.signup-container{
    height: fit-content;
    width: 315px;
    margin: auto;
    display: flex;
    flex-direction: column;
    flex-wrap: nowrap;
    border-radius: 10px;
    box-shadow: 1px 10px 10px 20px rgba(93, 96, 96, 0.433);
    align-items: center;
    
}

.signup-heading{
    width: 100%;
    height: 40px;
    background-color: blue;
    border-radius: 10px;
    padding: 5px;
}

.signup-heading h3{
    color: white;
    text-align: center;
    font-size: 25px;
}

.signup-form{
    padding: 15px;
}

.signup-form input{
    width: 100%;
    margin: 6px 0;
    outline: none !important;
    border-radius: 5px;
    padding: 6px 10px;
    background-color: rgba(0, 255, 255, 0.148);
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 15px;
}

.signup-form .signup-btn{
    width: 60%;
    padding: 5px 0;
    margin: 15px 20%;
    background-color: blue;
    color: white;
    cursor: pointer;
    border-radius: 5px;
    border: none;
    font-size: 18px;

}

.signup-form .signup-alternative{
    color: blue !important;
    font-size: 18px;
}


</style>