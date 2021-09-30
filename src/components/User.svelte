
<section>
    <div class="top-container">
        <div class="avatar">
            <img src="static/images/image-jeremy.png" alt="Jeremy Robson">
        </div>
        <div class="title">Report for</div>
        <div class="name">Jeremy <br> Robson</div>
    </div>
    
    <nav class="navigation">
        <a href="/">Daily</a>
        <a href="/weekly">Weekly</a>
        <a href="/monthly">Monthly</a>
    </nav>
</section>

<style>
    section {
        display: flex;
        flex-direction: column;
        height: 100%;
        width: 100%;
        max-width: 235px;
        margin: 0 30px 0 0;
        flex: .5;
    }

    section .top-container {
        position: relative;
        background-color: hsl(246, 80%, 60%);
        color: #fff;
        font-weight: 300;
        flex: 1;
        border-radius: 15px;
    }

    section .top-container .avatar {
        position: absolute;
        top: 30px;
        left: 30px;
        border-radius: 50%;
        border: 2px solid #fff;
        height: 80px;
        width: 80px;
    }

    section .top-container .avatar  img{
        width: 100%;
    }
    section .top-container .title{
        position: absolute;
        top: 150px;
        left: 30px;
        font-size: 14px;
        opacity: .7;
    }
    .top-container .name{
        position: absolute;
        top: 175px;
        left: 30px;
        font-size: 35px;
        letter-spacing: 0.03em;
    }
    .navigation {
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        padding: 25px 30px 0 30px;
        margin-top: -25px;
        flex: .5;
        background-color: hsl(235, 46%, 20%);
        border-radius: 15px;
    }
    .navigation a {
        color: #fff;
        text-decoration: none;
        opacity: .7;
        transition: opacity ease 150ms;
    }
    .navigation a:link:active, a:visited:active {
        opacity: 1;
    }
    .navigation a:hover {
        opacity: 1;
    }

    @media screen and (max-width: 768px) {
        section {
            display: block;
            flex-direction: column;
            max-width: 90%;
            margin: 0 0 30px 0;
        }

        section .top-container {
            height: 100%;
            height: 190px;
        }

        section .top-container .name {
            top: 80px;
            left: 40%;
        }

        section .top-container .title {
            top: 50px;
            left: 40%;
        }

        .navigation {
            flex-direction: row;
            height: 50px;
            align-items: center;
        }
    }
</style>
  