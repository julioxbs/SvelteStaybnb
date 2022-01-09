<div class="house-details">
    <div class="house-title">
        <h1>Wenge House</h1>

        <div class="row">
            <div>
                <i class="fas fa-star" />
                <i class="fas fa-star" />
                <i class="fas fa-star" />
                <i class="fas fa-star-half-alt" />
                <span>245 Reviews</span>
            </div>

            <div>
                <p>Location: San Francisco, California, United States</p>
            </div>
        </div>
    </div>

    <div class="gallery">
        <div><img src="/images/house-2.png" alt="house" /></div>
        <div><img src="/images/house-3.png" alt="house" /></div>
        <div><img src="/images/house-4.png" alt="house" /></div>
        <div><img src="/images/house-5.png" alt="house" /></div>
    </div>

    <div class="small-details">
        <h2>Entire rental unit hosted by Brandon</h2>
        <p>2 guest &nbsp; &nbsp; 2 beds &nbsp; &nbsp; 1 bathroom</p>
        <h4>$ 100 / day</h4>
    </div>

    <hr class="line" />

    <form class="check-form">
        <div>
            <label for="checkin">Check in</label>
            <input type="date" />
        </div>

        <div>
            <label for="checkin">Check out</label>
            <input type="date" />
        </div>

        <div class="guest-field">
            <label for="checkin">Guest</label>
            <input type="number" placeholder="2 Guest" max="2" />
        </div>

        <button type="submit">Check Availability</button>
    </form>

    <ul class="details-list">
        <li>
            Entire Home
            <span>You will have the entire flat for you.</span>
        </li>

        <li>
            Enhanced Clean
            <span>This host has committed to staybnb's cleaning process.</span>
        </li>

        <li>
            Great Location
            <span>90% of recent guests gave the location a 5 star rating.</span>
        </li>

        <li>
            Greate Check-in Experience
            <span
                >100% of recent guests gave the check-in process a 5 star
                rating.</span
            >
        </li>
    </ul>

    <hr class="line" />

    <p class="home-desc">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis nesciunt
        dolorum omnis exercitationem iusto rerum harum magnam laborum dolores
        est? Dolorum aliquam, esse aperiam nobis ipsam, quidem sequi sit non
        error facere dignissimos impedit earum fugit, minima repudiandae
        inventore? Non dolore nostrum rerum repellendus velit iure quaerat
        laboriosam, suscipit corporis, alias optio.
    </p>

    <hr class="line" />

    <div class="map">
        <h3>Location on map</h3>
        <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d20204.613622616893!2d-1.8609110078872926!3d50.72779180478887!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x48739f6a4356653f%3A0xfe754842a91c917e!2sBoscombe%2C%20Bournemouth!5e0!3m2!1spt-BR!2suk!4v1641731747859!5m2!1spt-BR!2suk"
            width="600"
            height="450"
            style="border:0;"
            allowfullscreen=""
            loading="lazy"
        />
        <b>Boscombe, Bournemouth, United Kingdom</b>
        <p>It's like a home away from home.</p>
    </div>

    <hr class="line" />

    <div class="host">
        <img src="/images/host.png" alt="people" />
        <div>
            <h2>Hosted by Brandon</h2>
            <p>
                <span>
                    <i class="fas fa-star" />
                    <i class="fas fa-star" />
                    <i class="fas fa-star" />
                    <i class="fas fa-star" />
                    <i class="fas fa-star-half-alt" />
                </span>&nbsp; &nbsp; 245 reviews &nbsp; &nbsp; response rate 100% &nbsp; &nbsp; Response time: 60 min
            </p>
        </div>
    </div>
</div>

<style>
    .house-details {
        padding: 0 12%;
    }

    .house-title {
        margin-top: 50px;
    }

    .house-title h1 {
        font-weight: 600;
    }

    .house-title .row {
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        margin: 10px 0;
    }

    .house-title span {
        margin: 0 20px;
    }

    .house-title i {
        color: #ff5361;
        font-size: 14px;
    }

    .gallery {
        display: grid;
        gap: 10px;
        grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    }

    .gallery div {
        max-width: 300px;
    }

    .gallery div img {
        width: 100%;
        border-radius: 10px;
    }

    .small-details h2 {
        font-weight: 500;
    }

    .small-details h4 {
        text-align: right;
        font-size: 22px;
    }

    .line {
        border: 0;
        height: 1px;
        background: #ccc;
        width: 100%;
        max-width: 800px;
        margin: 20px 0 50px;
    }

    .check-form {
        margin: 30px 0;
        background: #fff;
        box-shadow: 0 0 30px rgba(0, 0, 0, 0.3);
        border-radius: 8px;
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        padding: 10px 50px;
    }

    .check-form label {
        display: block;
    }

    .check-form div {
        padding: 20px;
    }

    .check-form input {
        background: transparent;
        border: 0;
        outline: none;
    }

    .check-form button {
        background: #ff5361;
        border: 0;
        outline: none;
        color: #fff;
        padding: 18px;
        width: max-content;
        border-radius: 8px;
        font-size: 16px;
    }

    .guest-field {
        flex: 1;
    }

    .details-list {
        margin: 50px 0;
        list-style: none;
    }

    .details-list li {
        margin-left: 50px;
        font-size: 20px;
        font-weight: 500;
        margin-bottom: 20px;
        color: #555;
    }

    .details-list li span {
        display: block;
        font-weight: 400;
        font-size: 16px;
    }

    .home-desc {
        max-width: 700px;
        margin-bottom: 50px;
    }

    .map {
        margin: 50px 0;
    }

    .map iframe {
        width: 100%;
        margin-bottom: 30px;
    }

    .map h3 {
        font-size: 26px;
        font-weight: 500;
        margin-bottom: 30px;
    }

    .map b {
        display: block;
    }

    .host {
        display: flex;
        align-items: center;
    }

    .host img {
        width: 80px;
        border-radius: 50%;
        margin-right: 30px;
    }

    .host h2 {
        margin-bottom: 10px;
        font-weight: 500;
    }

    .host i {
        color: #ff5361;
    }
</style>
