<script>
    import User from '../components/User.svelte'
</script>

<svelte:head>
    <link rel="stylesheet" href="css/main.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Rubik:wght@300;400;500&display=swap" rel="stylesheet">
</svelte:head>

<div class="container">
    <User />
    <div class="itemsContainer">
        <slot></slot>
    </div>
    <!-- <div class="attribution">
    Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
    Coded by <a href="#">Your Name Here</a>.
    </div> -->
</div>


<style>
    @import url('https://fonts.googleapis.com/css2?family=Rubik:wght@300;400;500&display=swap');
    .container {
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 100%;
        max-width: 1440px;
        height: 520px;
        font-family: 'Rubik', sans-serif;
    }

    .itemsContainer {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 245px 245px;
        flex-wrap: wrap;
        gap: 30px;
        flex: .6;
    }

    @media screen and (max-width: 768px) {
        .container {
            position: unset;
            top: 0;
            left: 0;
            transform: none;
            flex-direction: column;
            height: 100%;
        }
        .itemsContainer {
            display: flex;
            flex-direction: column;
            grid-template-columns: 1fr;
            grid-template-rows: 1fr;
            flex-wrap: nowrap;
            width: 90%;
        }
    }
/* 
    .attribution {
        position: absolute;
        bottom: -10%;
        font-size: 12px;
    } */
</style>