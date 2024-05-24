<script>
    let Title = "I-WINDOWS"
    let userName
    let password

</script>

<body>
    <div class="headContainer">
        <h2 class="title">{Title}</h2>
    </div>

    <br><br><br>

    <div class="bodyContainer">
        <div class="backDrop">
            <div class="dropHead">
                <p class="signHead"> Welcome Back </p>
                <p class=subText> Enter your credentials to continue.</p>
            </div>

            <div class="userCred">
                <label class="txtLabel" for="userName">Username: </label>
                <input class="inpBox" type="text" id="userName" placeholder="Enter your username here" bind:value={userName}>
            </div>

            <div class="passCred">
                <label class="txtLabel" for="userName">Password: </label>
                <input class="inpBox" type="password" id="password" placeholder="Enter your password here" bind:value={password}>
            </div>

            <div class="submitCont">
                <a href="/Home"><button class="submitBtn" type="button">Log In</button></a>
            </div>

            <div class="regCont">
                <span>Don't have an account?</span>
                <span class="regText">Register here</span>
            </div>

            <hr class="end">
        </div>

    </div>
</body>

<svelte:head>
    <style>
        html {
            max-width: 100%;
            min-height: 100%;
            background-color: #212429;
        }
    </style>
</svelte:head>

<style>
    .headContainer {
        align-self: center;
        max-width: 40%;
        height: 100px;
        margin: auto;
    }

    .bodyContainer {
        margin: auto;
    }

    .backDrop {
        position: relative;
        display: block;
        justify-content: center;
        border-radius: 60px;
        width: 60%;
        height: 620px;
        align-items: center;
        margin: auto;
        background: linear-gradient(white, white) padding-box, linear-gradient(90deg, #48d0b8, #9889f9) border-box;
        border: 6px solid transparent;
    }

    .signHead {
        color: #1e1e1e;
        font-size: 350%;
        position: relative;
        text-align: center;
        text-shadow: 0px 3px 2.5px #333333;
        margin: 12px 0 0 2px;
        font-family: 'Poppins', monospace;
    }

    .subText {
        font-family: 'Poppins';
        text-align: center;
        padding: 0 0 0 0;
        margin: -8px 0 0 0;
        font-size: 17px;
    }

    .userCred {
        width: auto;
        height: auto;
        margin-top: 8%;
        margin-bottom: 2%;
        text-align: center;
    }

    .txtLabel {
        color: #1e1e1e;
        font-family: 'Poppins';
        font-size: 26px;
        position: relative;
        margin: 3px 20px 3px 3px;
        top: 4px;
    }

    .inpBox {
        width: 530px;
        height: 25px;
        border-radius: 5px;
        font-family: 'Poppins';
        font-weight: bold;
        font-size: 15px;
        padding-left: 10px;
        color: #1e1e1e;
    }

    .inpBox::placeholder { /* Chrome, Firefox, Opera, Safari 10.1+ */
        font-family: 'Poppins';
        font-weight: lighter;
        opacity: 1; /* Firefox */
    }

    .passCred {
        width: auto;
        height: auto;
        text-align: center;
        margin-left: 0.79%;
        margin-bottom: 10%;
    }

    .submitCont {
        width: auto;
        height: auto;
        text-align: center;
        margin-bottom: 18px;
    }

    .submitBtn {
        border: none;
        background-color: #28586b;
        color: #F1F1F1;
        font-family: 'Poppins', monospace;
        text-align: center;
        font-size: 36px;
        size: 30px;
        width: 200px;
        height: 60px;
        border-radius: 14px;
        cursor: pointer;
        text-shadow: 3px 3px 5px #333333;
        box-shadow: 5px 6px 4px 0 rgba(0, 0, 0, 0.3);
        transition-duration: 0.4s;
    }

    .submitBtn:hover {
        background-color: #0f4253;
        color: #FFFFFF;
        text-shadow: 3px 3px 5px #333333;
        box-shadow: 5px 6px 4px 0 rgba(0, 0, 0, 0.3);
        cursor: pointer;
        font-family: 'Poppins', monospace;
        text-align: center;
        font-size: 36px;
        size: 30px;
        width: 200px;
        height: 60px;

    }

    .regCont {
        font-family: 'Poppins';
        text-align: center;
        width: auto;
        height: auto;
        margin-bottom: 70px;
    }

    .regText {
        font-weight: bold;
        color: #0f4253;
        text-decoration: underline;
    }

    .end {
        width: 750px;
        border-color: #1e1e1e;
        border-width: 1px;
    }

</style>