<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Crush</title>
    <link rel="stylesheet" href="vendor/css/style.css">
</head>
<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: 'Poppins', sans-serif;
        background-image: url('https://i.pinimg.com/736x/53/01/77/530177cc3518e6c9156becbcff11612a.jpg') , width : 100%;
    }
    html {
        font-size: 62.5%;
        line-height: 1.625rem;
        height: 100%;
        scroll-behavior: smooth;
    }

    :root {
        --white-color: #fff;
        --bg-main: #e3edf7;
        --bg-dark: #303234;
        --primary-color: #31344b;
        --text-color: #777777;
        --text-color-dark: #B0B3B8;
        --blue-color: #1877f2;
        --blue-color-2: #e9f5ff;
        --outer-shadow: 6px 6px 10px -1px rgba(0, 0, 0, 0.15),
        -6px -6px 10px -1px rgba(255, 255, 255, 0.7);
        --outer-shadow-o: 6px 6px 10px -1px rgba(0, 0, 0, 0.15),
        -6px -6px 10px -1px rgba(255, 255, 255, 0.7), inset 6px 6px 10px -1px rgba(0, 0, 0, 0.15),
        inset -6px -6px 10px -1px rgba(255, 255, 255, 0.7)
    ;
        --outer-shadow-dark: 6px 6px 10px -1px rgba(0, 0, 0, 0.3),
        -6px -6px 10px -1px rgba(255, 255, 255, 0.1);
        --outer-shadow-dark-o: 6px 6px 10px -1px rgba(0, 0, 0, 0.3),
        -6px -6px 10px -1px rgba(255, 255, 255, 0.1), inset 6px 6px 10px -1px rgba(0, 0, 0, 0.3),
        inset -6px -6px 10px -1px rgba(255, 255, 255, 0.1);
    }

    .app {
        width: 100%;
        height: 100vh;
        background-attachment: fixed;
        background: var(--bg-main);
        transition: all .3s linear;
        -moz-transition: all .3s linear;
        -webkit-transition: all .3s linear;
        -o-transition: all .3s linear;
    }
    .card {
        position: fixed;
        max-width: 350px;
        height: fit-content;
        display: flex;
        margin: auto;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        padding: 20px 12px;
        align-items: center;
        flex-direction: column;
        justify-content: center;
        background: var(--white-color);
        border-radius: 7px;
        background: var(--bg-main);
        box-shadow: var(--outer-shadow);
        transition: all .3s linear;
        -moz-transition: all .3s linear;
        -webkit-transition: all .3s linear;
        -o-transition: all .3s linear;
    }

    .card__title {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
    .card__title--name {
        position: relative;
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        margin-top: 10px;
    }
    .card__title--name h1 {
        position: relative;
        color: var(--primary-color);
        font-size: 2.2rem;
        font-weight: 600;
        line-height: 2.2rem;
        text-align: center;

    }

    .mt-10 {
        margin-top: 10px;
    }

    .row {
        width: 100%;
        display: flex;
        flex-wrap: wrap;
        margin-left: -5px;
        margin-right: -5px;
        justify-content: center;
    }
    .col {
        width: 100%;
        position: relative;
        padding-left: 5px;
        padding-right: 5px;
    }

    .button__list {
        position: relative;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-wrap: wrap;
    }
    .button {
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 15px 20px;
        text-align: center;
        background: var(--bg-main);
        box-shadow: var(--outer-shadow);
        color: var(--text-color);
        border: 2px solid var(--bg-main);
        font-size: 1.8rem;
        font-weight: 400;
        border-radius: 7px;
        transition: all .3s linear;
        -moz-transition: all .3s linear;
        -webkit-transition: all .3s linear;
        -o-transition: all .3s linear;
        cursor: pointer;
    }
    .button:hover {
        box-shadow: var(--outer-shadow-o);
        color: var(--blue-color) !important;
    }
    .col-lg-6 {
        flex: 0 0 50%;
        max-width: 50%;
    }

    @media screen and (max-width: 370px) {
        .mg-10 {
            margin: auto 10px;
        }

    }
    a
    {
        text-decoration: none;
        color: inherit;
    }
    .button__message::after
    {
        content: "Không";
    }

    .button__message:hover:after
    {
        content: "Vâng";
    }

    .col_third
    {
        color: red;
    }

    @keyframes heart
    {
        100%
        {
            transform: scale(1, 1);
        }

        50%
        {
            transform: scale(0.5, 0.5);
        }
    }
    #heart
    {
        animation-name: heart;
        animation-duration: 1s;
        animation-iteration-count: infinite;
    }
</style>
<body>
<div class="app">
    <div class="card mg-10" id="card1">
        <div class="card__title">
            <div class="col_third" id="heart">
                <i class="fa fa-heart fa-8x"></i>
            </div>
            <div class="card__title--name">
                <h1> Chúng ta hẹn hò nhé !!! </h1>
            </div>
        </div>
        <div class="button__list mt-10">
            <div class="row">
                <div class="col col-lg-6 mt-10">
                    <div class="button button__subscribe btnNo" onclick="showMess()">
                        <span>Em đồng ý</span>
                    </div>
                </div>
                <div class="col col-lg-6 mt-10">
                    <div class="button button__message btnNo" onclick="showMess()">
                        <span></span>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="card mg-10" id="card2" style="display: none;">
        <div class="card mg-10">
            <div style="height: 30px;"></div>
            <div class="card__title--name">
                <h1>
                    <span style="color: red;">Cảm ơn em </span>
                    <br> vì đã cho anh cơ hội được làm người yêu em <br>
                    <span> anh mong rằng chúng ta sẽ tiến tới cánh cửa hôn nhân . </span>
                </h1>
            </div>
            <div style="height: 30px;"></div>
        </div>
    </div>
</div>

<script >
    function showMess()
    {
        document.getElementById("card1").style.display = 'none';
        document.getElementById("card2").style.display = "inline";
    }
</script>
</body>
</html>
