<script>
    export let title
    export let current
    export let previous
    export let color
    export let image
</script>

<section class="item-container">
    <div class="top-image" style="background-color: {color}">
        <img src="{image}" alt="">
    </div>
    <div class="title">{title}</div>
    <div class="timeframes">
        <div class="current">{current}hrs</div>
        <div class="previous">Last Week - {previous}hrs</div>
    </div>
</section>

<style>
    section {
        display: flex;
        flex-direction: column;
        height: calc(100% - 50px);
        margin-top: 45px;
        background-color: hsl(235, 46%, 20%);
        border-radius: 15px;
        font-weight: 300;
    }

    .top-image {
        height: 50px;
        margin-top: -45px;
        height: 60px;
        border-radius: 15px 15px 0 0;
        z-index: -1;
        overflow: hidden;
    }

    .top-image img {
        float: right;
        margin-top: -5px;
    }

    .title {
        padding: 30px 30px 15px 30px;
    }
    .timeframes {
        padding: 0 30px;
    }
    .current {
        font-size: 50px;
    }

    @media screen and (max-width: 768px) {
        .timeframes {
            display: flex;
            flex-direction: row;
            align-items: center;
            justify-content: space-between;
        }
    }
</style>