# test_vibo_and_reponsive

<!DOCTYPE html>
<html lang="vn,en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://fonts.googleapis.com/css?family=Open+Sans|Roboto+Condensed|Work+Sans&display=swap" rel="stylesheet">
    <title>Vibo</title>
    <style type="text/css">
        *{
            margin: 0;
            padding:0;
            border: 0;
            text-decoration: none;
            box-sizing: border-box;
        }

        .clearfix:after{
            content:' ';
            display: table;
            clear: both;
        }

        p.paragraphs{
            font-size: 14px;
            font-weight: normal;
            line-height: 27px;
        }

        h2.heading_2{
            font-size: 30px;
            font-weight: normal;
            font-family: 'Open Sans', sans-serif;
            line-height: 60px;
            color: #233148;
        }

        li{
            list-style: none;
        }

        #hero{
            height: 1000px;
            background: linear-gradient(to bottom, #0abdf2, #0ed0f0);
            background-image: url(image/ware.png), url(image/phone.png), url(image/BG.png);
            background-repeat: no-repeat, no-repeat, no-repeat;
            background-position: center bottom, center bottom -89px, center center;
            background-size: 101% auto, auto, cover;
        }
        /*Container*/
        div.container{
            max-width: 1170px;
            margin: 0px auto;
        }
        /*Header*/
        #hero #header{
            height: 50px;
            padding-top: 46px;
        }

        #hero #header >a{
            float: left;
        }

        #hero #header >ul{
            float: right;
        }

        #hero #header >ul >li{
            display: inline-block;
        }

        #hero #header ul li a{
            font-family: 'Roboto Condensed', sans-serif;
            display: block;
            color: white;
            font-size: 16px;
            line-height: 44px;
            padding:0 20px;
        }

        #hero #header ul li a:hover{
            text-decoration: underline;
        }
        /*Intro*/
        #hero #intro h1,
        #hero #intro h2{
            color: white;
        }

        #hero #intro h1{
            margin-top: 115px;
            text-align: center;
            font-size: 45px;
            line-height: 60px;
            padding: 0px 300px;
            font-family: 'Work Sans', sans-serif;
            font-weight: normal;
        }

        #hero #intro h2{
            text-align: center;
            font-family: 'Open Sans', sans-serif;
            font-weight: normal;
            font-size: 15px;
            line-height: 28px;
            padding:0px 300px;
            margin-top: 20px;
        }
        /*LINK*/
        #hero #link{
            text-align: center;
            margin-top: 58px;
        }

        #hero #link a{
            display: inline-block;
            height: 40px;
            line-height: 40px;
            color: #233148;
            padding: 0px 30px;
            border: 1px solid white;
            border-radius: 6px;
        }

        #hero #link a:first-child{
            background-color: white;
        }

        #hero #link a:nth-child(2){
            color: white;
        }
        /*App-datail*/
        #app-detail{
            background-color: #fafafc;
            padding-bottom: 144px;
        }

        #app-detail div.container >img{
            float: left;
            margin-left: 108px;
            margin-top: 284px;
        }

        #app-detail div.container > div{
            float: right;
            width: 800px;
            margin-top: 114px;
            position: relative;
        }

        #app-detail div.container > div > div{
            padding: 30px;
            width: 270px;
            background-color: white;
            box-shadow: /*Spread*/0px /*Disance*/6px /*Size*/9px rgba(35, 39, 47, 0.1);
            position: absolute;
        }

        #app-detail div.container > div > div:nth-child(1){
            left: 139px;
        }

        #app-detail div.container > div > div:nth-child(2){
            top: 97px;
            left: 469px;
        }

        #app-detail div.container > div > div:nth-child(3){
            top: 394px;
            left: 72px;
        }

        #app-detail div.container > div > div:nth-child(4){
            top: 518px;
            left: 442px;
        }

        #app-detail div.container > div > div > img{
            display: block;
            margin: 28px auto 15px auto;
        }

        #app-detail div.container > div > div h3{
            text-align: center;
            font-family: 'Roboto Condensed', sans-serif;
            font-size: 14px;
            font-weight: normal;
            line-height: 27px;
            color: #233148; 
            padding: 10px 0px;
        }

        #app-detail div.container > div > div p{
            text-align: center;
            color: #6a6d89;
        }
        /*STABLE*/
        #stable{
            padding: 110px 0px;
            height: 626px;
            background-color: white;
        }

        #stable div.container > div{
            width: 472px;
            float: left;
        }

        #stable div.container > div > h2{
            text-align: right;
            margin-bottom: 31px;/*(lấy khoảng cách h2 lineheight-fontsize(60-30=30/2=15),lấy khoảng cách p lineheight-fontsize(27-14=13/2=6),(15=6=21,rồi lấy khoảng cách đo đc =52,52-21=31))
*/      }

        #stable div.container > div > p{
            text-align: right;
            color: #6a6d89;
            margin-bottom: 52px;/*(lấy khoảng cách p lineheight-fontsize(27-14=13/2=6),đo tới cái div của a khoảng cách bằng 58, lấy 58-6=52)*/
        }

        #stable div.container > div > div{
            text-align: right;
        }

        #stable div.container > div > div > a{
            display: inline-block;
            padding: 0px 43px;
            font-size: 15px;
            font-weight: normal;
            height: 50px;
            line-height: 50px;
            background-color: #33d2fd;
            border-radius: 6px;
            color: white;
        }

        ul#stable-list{
            width: 570px;
            float: right;
        }

        ul#stable-list > li{
            margin-bottom: 20px;
            box-shadow: /*Spread*/0px /*Disance*/6px /*Size*/9px rgba(35, 39, 47, 0.1);
            min-height: 75px;
            transition: background-color 1s ease-in, height 0.5s ease-in;
        }

        ul#stable-list > li >a{
            display: block;
            height: 75px;
            line-height: 75px;
            /*background-color: white;*/
            color: #3e485a;
            padding-left: 90px;
            background-repeat: no-repeat;
            background-position: 32px center;
        }

        ul#stable-list  > li:nth-child(1) > a{
            background-image: url(image/icons/love.png);
        }

        ul#stable-list  > li:nth-child(2) > a{
            background-image: url(image/icons/mouse.png);
            background-position: 38px center;
        }

        ul#stable-list  > li:nth-child(3) > a{
            background-image: url(image/icons/briefcase.png);
        }

        ul#stable-list  > li:nth-child(4) > a{
            background-image: url(image/icons/pencil.png);
        }

        ul#stable-list > li > p {
            display: none;
            color: white;
            padding: 0px 90px 30px 90px;

        }

        ul#stable-list li:hover{
            background-color: #33d2fd;
        }

        ul#stable-list li:hover > p{
            display: block;

        }
        /*FREATURES*/
        #freatures{
            background-color: #fafafc;
            padding: 70px 0px;
        }

        #freatures div.container > img {
            float: left;
            display: block;
        }

        #freatures div.container > div {
            width: 470px;
            float: right;
        }

        #freatures div.container > div > h2{
            text-align: left;
            padding-left: 35px;
        }

        #freatures div.container > div  ul li{
            background: transparent url(image/icons/checked.png) no-repeat left center;
            padding-left: 35px;
            font-size: 15px;
            font-weight: normal;
            line-height: 45px;
            color: #233148;
        }

        #freatures div.container > div p{
            text-align: left;
            margin-top: 32px;
        }
        /*GET-APP*/
        #get-app {
            background: linear-gradient(to bottom, #0abdf2, #0ed0f0);
            background: url(image/BG.png) no-repeat center center;
            padding: 110px 0px;
            position: relative;
        }

        #get-app div.container > img{
            float: left;
            margin-left: 175px;
        }

        #get-app div.container > div#get-app-info{
            float: right;
            width: 470px;
            margin-right: 100px;
        }

        #get-app div.container > div#get-app-info >h2{
            text-align: left;
            color: #233148;
            font-family: 'Open Sans', sans-serif;
            font-size: 30px;
            font-weight: normal;
            line-height: 60px;
            margin-top: 155px;
            margin-bottom: 20px;
        }

        #get-app div.container > div#get-app-info >p{
            text-align: left;
            color: white;
            margin-bottom: 60px;
        }

        #get-app div.container > div#get-app-info div a{
            padding-right: 37px;
        }

        #get-app div.container a#get-app-btn{
            display: inline-block;
            text-align: center;
            background: linear-gradient( to bottom, #fc6573, #f8447b);
            width: 370px;
            height: 70px;
            text-transform: uppercase;
            font-size: 20px;
            font-weight: normal;
            line-height: 70px;
            color: white;
            position: absolute;
            bottom: -35px;
            left: 50%;
            margin-left: -185px;
            box-shadow: 0px 11px 29px rgba(225, 7, 95, 0.2)
        }
        /*LINKS*/
        #links{
            padding-top: 140px;
            padding-bottom: 40px;
        }

        #links div.container > div{
            float: left;
            width: 170px;
            margin-right: 32px;
        }

        #links div.container > div:first-child{
            margin-left: 200px;
        }

        #links div.container div h4{
            font-family: 'Open Sans', sans-serif;
            font-size: 15px;
            font-weight: normal;
            line-height: 27px;
            color: #233148;
            margin-bottom: 17px;
        }

        #links div.container > div ul li a{
            display: block;
            font-size: 14px;
            font-weight: normal;
            line-height: 27px;
            color: #6a6d89;
        }

        #links div.container > div ul li a:hover{
            color: black;
        }
        /*GET-IN-TOUCH*/
        #get-in-touch{
            padding-top: 40px;/*(dòng 396(uầy cái này hơi khó giải thích-tuy ở chung một div nhưng nó chia ra một khoảng trắng lớn(là 80px chỗ khoảng trắng).Nếu mà là một trang web khi các bạn scoll thì cái khoảng mà các bạn đặt mỗi cái 40px(bottom=40px-top=40px cho mỗi element)nó sẽ tạo ra một khoảng trắng 40px giúp cái elemet đó nhìn rõ hơn(nếu không chia 2 khoảng trắng or nếu các bạn đặt element trên or dưới là 80px thì khi trang web hoạt động, scoll trang nó sẽ gấy ra sự khó chịu cho người xem) ))*/
            padding-bottom: 87px;
        }

        #get-in-touch div.container h2{
            text-align: center;
            margin-bottom: 7px;

        }

        #get-in-touch div.container p{
            text-align: center;
            color: #6a6d89;
            margin-bottom: 68px;

        }

        #get-in-touch div.container form{
            text-align: center;
        }

        #get-in-touch div.container form > input{
            display: inline-block;
            width: 568px;
            height: 50px;
            background-color: #f6f7fb;
            border: none;
            font-size: 14px;
            padding: 0px 18px;
        }

        #get-in-touch div.container form > input:focus{/*(làm mất viền của input)*/
            outline: none;
        }

        #get-in-touch div.container form > button{
            display: inline-block;
            width: 170px;
            height: 50px;
            background-color: #33d2fd;
            color: #233148;
            font-size: 15px;
            font-weight: normal;
            line-height: 50px;
            border: none;
            cursor: pointer;
            margin-left: 32px;
        }
        /*FOOTER*/
        #footer{
            background-color: #233148;
        }

        #footer div.container p{
            float: left;
            font-size: 14px;
            line-height: 100px;
            color: white;
        }

        #footer div.container  ul{
            float: right;
        }

        #footer div.container  ul li{
            display: inline-block;
            line-height: 100px;
        }

        #footer div.container  ul li a{
            display: block;
            padding: 0 22px;
        }

        #footer div.container  ul li a:hover img{
            transform: scale(1);
            transition: transform 0.3s ease-in;
        }

        /*--RESPONSIVE--*/
        /*> 960px screen*/
        @media screen and (min-width: 960px) and (max-width: 1169px){
            .container{
                padding-left: 15px;
                padding-right: 15px;
            }
            /*HERO*/
            #hero #header > a{
                padding-left: 20px;
            }

            #hero #intro h1 {
                margin-top: 50px;
                text-align: center;
                font-size: 45px;
                line-height: 60px;
                font-family: 'Work Sans', sans-serif;
                font-weight: normal;
                padding: 0px;
            }
            /*APP_DETAIL*/
            #app-detail {
                background-color: #fafafc;
                padding-bottom: 210px;
            }

            #app-detail div.container >img {
                float: left;
                margin-left: 30px;
                margin-top: 70px;
            }

            #app-detail div.container > div {
                float: right;
                width: 555px;
                margin-top: 60px;
                position: relative;
            }

            #app-detail div.container > div > div {
                padding: 30px;
                width: 230px;
                background-color: white;
                box-shadow: /*Spread*/0px /*Disance*/6px /*Size*/9px rgba(35, 39, 47, 0.1);
                position: absolute;
            }

            #app-detail div.container > div > div:nth-child(1) {
                left: 0px;
                top: 0px;
            }

            #app-detail div.container > div > div:nth-child(2) {
                top: 69px;
                left: 279px;
            }

            #app-detail div.container > div > div:nth-child(3) {
                top: 377px;
                left: -42px;
            }

            #app-detail div.container > div > div:nth-child(4) {
                top: 450px;
                left: 313px;
            }
            /*STABLE*/
            #stable {
                padding: 80px 0px;
                height: 581px;
                background-color: white;
            }

            #stable div.container > div {
                width: 327px;
                float: left;
            }

            #stable div.container > div > h2 {
                text-align: center;
                margin-bottom: 31px;
            }

            #stable div.container > div > p {
                text-align: center;
                color: #6a6d89;
                margin-bottom: 52px;
            }

            #stable div.container > div > div {
                text-align: center;
            }

            ul#stable-list {
                width: 540px;
                float: right;
            }
            /*FREATURES*/
            #freatures div.container > img {
                float: left;
                display: block;
                height: 300px;
            }

            #freatures div.container > div {
                width: 420px;
                float: right;
            }
            /*GET-APP*/
            #get-app{
                padding-bottom: 110px;
            }

            #get-app div.container > img {
                float: left;
                margin-left: 15px;
            }

            #get-app div.container > div#get-app-info {
                float: right;
                width: 430px;
                margin-right: 100px;
            }
            /*LINKS*/
            #links div.container > div:first-child {
                margin-left: 117px;
            }

        }

        @media screen and (min-width: 768px) and (max-width: 959px){
            /*HERO*/
            #hero {
                height: 940px;
                background: linear-gradient(to bottom, #0abdf2, #0ed0f0);
                background-image: url(image/ware.png), url(image/phone.png), url(image/BG.png);
                background-repeat: no-repeat, no-repeat, no-repeat;
                background-position: center bottom, center bottom -89px, center center;
                background-size: 100% auto, auto, cover;
}

            #hero #header > a{
                padding-left: 20px;
            }

            #hero #intro h1 {
                margin-top: 60px;
                text-align: center;
                font-size: 45px;
                padding: 0px;
                line-height: 60px;
                font-family: 'Work Sans', sans-serif;
                font-weight: normal;
            }

            #hero #intro h2 {
                text-align: center;
                font-family: 'Open Sans', sans-serif;
                font-weight: normal;
                font-size: 15px;
                line-height: 28px;
                margin-top: 20px;
                padding: 0px;
            }
            /*APP-DETAIL*/
            #app-detail {
                background-color: #fafafc;
                padding-bottom: 560px;
            }

            #app-detail div.container >img {
                display: none;
            }

            #app-detail div.container > div {
                padding-top: 20px;
                position: relative;
                margin-top: 0px;
            }

            #app-detail div.container > div > div {
                padding: 10px;
                width: 520px;
                background-color: white;
                box-shadow: /*Spread*/0px /*Disance*/6px /*Size*/9px rgba(35, 39, 47, 0.1);
                position: absolute;
            }

            #app-detail div.container > div > div:nth-child(1) {
                left: 60px;
            }

            #app-detail div.container > div > div:nth-child(2) {
                top: 160px;
                left: 132px;
            }

            #app-detail div.container > div > div:nth-child(3) {
                top: 300px;
                left: 210px;
            }

            #app-detail div.container > div > div:nth-child(4) {
                top: 440px;
                left: 280px;
            }

            #app-detail div.container > div > div > img {
                display: block;
                margin: 35px 10px 0px auto;
                float: left;
            }

            #app-detail div.container > div > div h3 {
                text-align: center;
                font-family: 'Roboto Condensed', sans-serif;
                font-weight: normal;
                font-size: 20px;
                line-height: 27px;
                color: #233148;
                padding: 10px 0px;
            }

            #app-detail div.container > div > div p {
                text-align: left;
                color: #6a6d89;
            }
            /*STABLE*/
            #stable {
                padding: 20px 0px;
                height: 710px;
                background-color: white;
            }

            #stable div.container > div {
                width: auto; 
                float: none; 
            }

            #stable div.container > div > h2 {
                text-align: center;
                margin-bottom: 20px;
            }

            #stable div.container > div > p {
                text-align: center;
                color: #6a6d89;
                margin-bottom: 20px;
                padding: 0px 20px;
            }

            #stable div.container > div > div {
                text-align: center;
            }

            ul#stable-list {
                width: 730px;
                margin-left: 20px;
                float: none;
                margin-top: 20px;
            }

            ul#stable-list > li {
                margin-bottom: 20px;
                box-shadow: /*Spread*/0px /*Disance*/6px /*Size*/9px rgba(35, 39, 47, 0.1);
                min-height: 75px;
                transition: background-color 1s ease-in, height 0.5s ease-in;
            }
            /*FREATURES*/
            #freatures {
                background-color: #fafafc;
                padding: 20px 0px;
            }

            #freatures div.container > img {
                width: 440px;
                display: block;
                margin: 0px 170px;
            }

            #freatures div.container > div {
                width: auto;
                float: none;
            }

            #freatures div.container > div > h2 {
                text-align: center;
                padding-left: 0px;
            }

            #freatures div.container > div ul li {
                background: transparent url(image/icons/checked.png) no-repeat left center;
                padding-left: 35px;
                font-size: 15px;
                font-weight: normal;
                line-height: 45px;
                color: #233148;
                margin-left: 325px;
            }

            #freatures div.container > div p {
                text-align: center;
                margin-top: 20px;
                padding: 0px 20px;
            }
            /*GET-APP*/
            #get-app {
                background: linear-gradient(to bottom, #0abdf2, #0ed0f0);
                background: url(image/BG.png) no-repeat center center;
                padding: 20px 0px;
                position: relative;
            }

            #get-app div.container > img {
                float: none;
                margin-left: 175px;
                padding-top: 10px;
                display: none;
            }

            #get-app div.container > div#get-app-info {
                float: none; 
                width: auto; 
                margin-right: 0px; 
            }

            #get-app div.container > div#get-app-info >h2 {
                text-align: center;
                color: #233148;
                font-family: 'Open Sans', sans-serif;
                font-size: 30px;
                font-weight: normal;
                line-height: 60px;
                margin-top: 20px;
                margin-bottom: 20px;
            }

            #get-app div.container > div#get-app-info >p {
                text-align: center;
                color: white;
                margin-bottom: 20px;
                padding: 0px 20px;
            }

            #get-app div.container > div#get-app-info div{
                text-align: center;
                padding-bottom: 40px;
            }

            #get-app div.container > div#get-app-info div a {
                padding-right: 37px;
            }
            /*LINKS*/
            #links {
                padding-top: 100px;
                padding-bottom: 0px;
            }

            #links div.container > div:first-child {
                margin-left: 31px;
            }

            #links div.container > div {
                float: left;
                width: 130px;
                margin-right: 0px;
                margin: 0px 31px;
            }

            #links div.container div h4 {
                font-family: 'Open Sans', sans-serif;
                font-size: 15px;
                font-weight: normal;
                line-height: 27px;
                color: #233148;
                margin-bottom: 17px;
            }
            /*GET-IN-TOUCH*/
            #get-in-touch div.container form > input {
                display: inline-block;
                width: 550px;
                height: 50px;
                background-color: #f6f7fb;
                border: none;
                font-size: 14px;
                padding: 0px 18px;
            }
        }
    </style>
</head>
<body>
    <div id="hero">
        <div class="container">
            <div id="header">
                <a href="#">
                    <img src="image/Logo.png"/>
                </a>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Apps</a></li>
                    <li><a href="#">Info</a></li>
                </ul>
            </div>
            <div class="clearfix"></div>
            <div id="intro">
                <h1>Chosse a better way to represent your app</h1>
                <h2>Lorem ipsum dolor sit amet consectetur adipisicing elit!</h2>
            </div>
                <div id="link">
                <a href="#">Download Free</a>
                <a href="#">Contact Us</a>
                </div>
        </div>
    </div>
            <div id="app-detail">
                <div class="container">
                    <img src="image/phone.png"/>
                    <div>
                        <div>
                            <img src="image/icons/maket.png"/>
                            <h3 class="heading_3">First 7 Days free</h3>
                            <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elit Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
                        </div>
                        <div>
                            <img src="image/icons/text.png"/>
                            <h3 class="heading_3">Fully Support</h3>
                            <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elit! Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
                        </div>
                        <div>
                            <img src="image/icons/paint.png"/>
                            <h3 class="heading_3">Modern Flat Design</h3>
                            <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elit! Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
                        </div>
                        <div>
                            <img src="image/icons/phones.png"/>
                            <h3 class="heading_3">User Friendly</h3>
                            <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elit! Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
                        </div>
                    </div>
                </div>
                <div class="clearfix"></div>
            </div>
            <div>
                <div id="stable">
                    <div class="container">
                        <div>
                            <h2 class="heading_2">Stable And ready</h2>
                            <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elitLorem ipsum dolor sit amet consectetur adipisicing elit Lorem ipsum dolor sit amet consectetur adipisicing elit Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
                        <div>
                            <a href="#">Download Free</a>
                        </div>
                        </div>
                            <ul id="stable-list">
                                <li>
                                    <a href="#">Made With Love</a>
                                    <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elitLorem ipsum dolor consectetur adipisicing elitLorem ipsum dolor</p>
                                </li>
                                <li>
                                    <a href="#">Free of Use</a>
                                    <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elitLorem ipsum dolor consectetur adipisicing elitLorem ipsum dolor</p>
                                </li>
                                <li>
                                    <a href="#">Fully Support Avaliable</a>
                                    <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elitLorem ipsum dolor consectetur adipisicing elitLorem ipsum dolor</p>
                                </li>
                                <li>
                                    <a href="#">Flat and Modem Ui & Ux</a>
                                    <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elitLorem ipsum dolor consectetur adipisicing elitLorem ipsum dolor</p>
                                </li>
                            </ul>
                    </div>
                </div>
        <div id="freatures">
            <div class="container">
                <img src="image/code.png"/>
                <div>
                    <h2 class="heading_2">Everything You Need</h2>
                    <ul>
                        <li>Android</li>
                        <li>Iphone</li>
                    </ul>
                    <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elitLorem ipsum dolor Lorem ipsum dolor sit amet consectetur adipisicing elit Lorem ipsum dolor sit amet consectetur adipisicing elit Lorem ipsum dolor sit amet consectetur adipisicing elit!</p>
                </div>
            </div>
            <div class="clearfix"></div>
        </div>
        <div id="get-app">
            <div class="container">
                <img src="image/phone.png">
                <div id="get-app-info">
                    <h2 class="heading_2">Now Avalible</h2>
                    <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elitLorem ipsum dolor Lorem ipsum dolor sit amet consectetur adipisicing elit Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
                    <div>
                        <a href="#"><img src="image/icons/appstore.png"></a>
                        <a href="#"><img src="image/icons/googleplay.png"></a>
                    </div>
                </div>
                    <a id="get-app-btn" href="#">Get The App Today</a>
            </div>
            <div class="clearfix"></div>
        </div>
        <div id="links">
            <div class="container">
                <div>
                    <h4>Company</h4>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Press</a></li>
                    </ul>
                </div>
                <div>
                    <h4>Development</h4>
                    <ul>
                        <li><a href="#">IOS</a></li>
                        <li><a href="#">Android</a></li>
                    </ul>
                </div>
                <div>
                    <h4>Community</h4>
                    <ul>
                        <li><a href="#">Social</a></li>
                        <li><a href="#">Forum</a></li>
                        <li><a href="#">Contact</a></li>
                        <li><a href="#">FAQ</a></li>
                    </ul>
                </div>
                <div>
                    <h4>Info</h4>
                    <ul>
                        <li><a href="#">Terms of Service</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="clearfix"></div>
        <div id="get-in-touch">
            <div class="container">
                <h2 class="heading_2">Get In Touch</h2>
                <p class="paragraphs">Lorem ipsum dolor sit amet consectetur adipisicing elitLorem ipsum dolor</p>
                <form>
                    <input type="text" name="email">
                    <button type="submit">Count Me In</button>
                </form>
            </div>
        </div>
        <div id="footer">
            <div class="container">
                <p>&copy; 2018 - Appo,All Right Reserved</p>
                <ul>
                    <li><a href="#"><img src="image/icons/Facebook.png"/></a></li>
                    <li><a href="#"><img src="image/icons/Twitter.png"/></a></li>
                    <li><a href="#"><img src="image/icons/Dribble.png"/></a></li>
                    <li><a href="#"><img src="image/icons/Google.png"/></a></li>
                    <li><a href="#"><img src="image/icons/Youtube.png"/></a></li>
                </ul>
            </div>
            <div class="clearfix"></div>
        </div>
</body>
</html>
