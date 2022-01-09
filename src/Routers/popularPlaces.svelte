<script>
    let photos = [
        { src: "/images/image-1.png", title: "London" },
        { src: "/images/image-2.png", title: "Switzerland" },
        { src: "/images/image-3.png", title: "Australia" },
        { src: "/images/image-4.png", title: "France" },
        { src: "/images/image-5.png", title: "Amsterdam" },
        { src: "/images/image-6.png", title: "Netherlands" },
        { src: "/images/image-7.png", title: "New York" },
        { src: "/images/image-8.png", title: "Chicago" },
        { src: "/images/image-9.png", title: "San Francisco" },
        { src: "/images/image-10.png", title: "Shanghai" },
    ];

    let trendPhotos = [
        {src: "/images/dubai.png", title: "Dubai"},
        {src: "/images/new-york.png", title: "New York"},
        {src: "/images/paris.png", title: "Paris"},
        {src: "/images/new-delhi.png", title: "New Delhi"},
    ]
</script>

<div class="container">
    <h2 class="sub-title">Exclusives</h2>
    <div class="exclusives">
        {#each photos as { src, title }}
            <div>
                <img {src} alt={title} />
                <span>
                    <h3>{title}</h3>
                    <p>Start $250</p>
                </span>
            </div>
        {/each}
    </div>

    <h2 class="sub-title">Trending Places</h2>
    <div class="trending">
        {#each trendPhotos as {src, title}}
            <div>
                <img src="{src}" alt="{title}">
                <h3>{title}</h3>
            </div>
        {/each}
    </div>

    <div class="cta">
        <h3>Sharing <br> Is Earning Now</h3>
        <p>
            Great opportunity to make money by <br> sharing your extra space.
        </p>
        <button class="cta-btn">know More</button>
    </div>

    <h2 class="sub-title">Travellers Stories</h2>
    <div class="stories">
        <div>
            <img src="/images/story-1.png" alt="stories">
            <p>Popular European countries with a buget of just $10,000</p>
        </div>

        <div>
            <img src="/images/story-2.png" alt="stories">
            <p>Popular European countries with a buget of just $10,000</p>
        </div>

        <div>
            <img src="/images/story-3.png" alt="stories">
            <p>Popular European countries with a buget of just $10,000</p>
        </div>
    </div>

    <button class="start-btn">Start making money</button>

    <div class="about-msg">
        <h2>About Staybnb</h2>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis minima voluptatum facere natus doloribus! Velit enim dignissimos, ex cumque repellendus laboriosam natus veritatis sapiente officiis, impedit soluta iste? Officia architecto aliquid dicta magnam. Deserunt totam fugiat iusto consequuntur itaque necessitatibus quidem dolores optio dolorem aliquam ipsa, corporis nobis praesentium illum suscipit molestiae enim eos quia unde.
        </p>
    </div>
</div>

<style>
    .exclusives {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 30px;
    }

    .exclusives div img {
        width: 100%;
        border-radius: 10px;
    }

    .exclusives div {
        position: relative;
    }

    .exclusives div span {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: center;
        color: #fff;
    }

    .trending {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 30px;
        margin-bottom: 30px;
    }

    .trending div img {
        width: 100%;
        border-radius: 10px;
    }

    .trending h3 {
        font-weight: 300;
        margin-top: 10px;
    }

    .cta {
        margin: 80px 0;
        background-image: linear-gradient(to right, #3f2321, transparent), url("/images/banner-2.png");
        background-size: cover;
        background-position: center;
        border-radius: 10px;
        padding: 5%;
        color: #fff;
    }

    .cta h3 {
        font-size: 4vw;
        line-height: 5.3vw;
        font-weight: 500;
    }

    .cta p {
        font-size: 18px;
        margin: 10px 0;
    }

    .cta-btn {
        background: #ff5361;
        border: 0;
        cursor: pointer;
        color: #fff;
        padding: 12px 30px;
        border-radius: 8px;
        margin-top: 20px;
        text-transform: uppercase;
    }

    .stories {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 30px;
    }

    .stories div img {
        width: 100%;
        border-radius: 10px;
    }

    .stories div {
        position: relative;
        text-align: center;
    }

    .stories p {
        width: 80%;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: #fff;
        font-size: 26px;
    }

    .start-btn {
        border: 0;
        background: #ff5361;
        color: #fff;
        width: 80%;
        max-width: 350px;
        display: block;
        margin: 60px auto;
        padding: 15px;
        border-radius: 30px;
        font-size: 20px;
    }

    .about-msg {
        text-align: center;
        border: 2px solid hsl(355, 100%, 66%);
        padding: 12px 8px;
        margin: 12px 0;
    }

    .about-msg h2 {
        text-transform: uppercase;
        color: #333;
        margin: 12px 0;
    }
</style>
