<script>
    let photos = [
        { url: "/images/image-s1.png" },
        { url: "/images/image-s2.png" },
        { url: "/images/image-s3.png" },
        { url: "/images/image-s4.png" },
        { url: "/images/image-s5.png" },
        { url: "/images/image-s6.png" },
    ];
</script>

<div class="list-container">
    <div class="left-col">
        <p>200+ Options</p>
        <h1>Recommended Places In San Francisco</h1>
        {#each photos as { url }}
            <div class="house">
                <div class="house-img">
                    <img src="{url}" alt="house" />
                </div>

                <div class="house-info">
                    <p>Private Villa in San Francisco</p>
                    <h3>Deluxe Queen Room With Street View</h3>
                    <p>1 Bedroom / 1 Bathroom / Wifi / Kitchen</p>
                    <i class="fas fa-star" />
                    <i class="fas fa-star" />
                    <i class="fas fa-star" />
                    <i class="fas fa-star-half-alt" />
                    <div class="house-price">
                        <p>2 Guest</p>
                        <h4>$100 / day</h4>
                    </div>
                </div>
            </div>
        {/each}
    </div>

    <div class="right-col">
        <div class="sidebar">
            <h2>Select Filters</h2>
            <h3>Property Type</h3>
            <div class="filter">
                <input type="checkbox"> <p>House</p> <span>(0)</span>
            </div>

            <div class="filter">
                <input type="checkbox"> <p>Hostel</p> <span>(0)</span>
            </div>

            <div class="filter">
                <input type="checkbox"> <p>Flat</p> <span>(0)</span>
            </div>

            <div class="filter">
                <input type="checkbox"> <p>Villa</p> <span>(0)</span>
            </div>

            <div class="filter">
                <input type="checkbox"> <p>Guest Suit</p> <span>(0)</span>
            </div>

            <h3>Amenities</h3>

            <div class="filter">
                <input type="checkbox"> <p>Air Conditioning</p> <span>(0)</span>
            </div>

            <div class="filter">
                <input type="checkbox"> <p>Wifi</p> <span>(0)</span>
            </div>

            <div class="filter">
                <input type="checkbox"> <p>Gym</p> <span>(0)</span>
            </div>

            <div class="filter">
                <input type="checkbox"> <p>Pool</p> <span>(0)</span>
            </div>

            <div class="filter">
                <input type="checkbox"> <p>Kitchen</p> <span>(0)</span>
            </div>

            <div class="sidebar-link">
                <a href="#">View More</a>
            </div>
        </div>
    </div>

    <div class="pagination">
        <img src="/images/arrow.png" alt="arrow">
        <span>1</span>
        <span>2</span>
        <span>3</span>
        <span>4</span>
        <span>5</span>
        <span>&middot; &middot; &middot; &middot;</span>
        <span>20</span>
        <img src="/images/arrow.png" alt="arrow">
    </div>
</div>

<style>
    .list-container {
        margin-top: 50px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    .left-col {
        flex-basis: 70%;
    }

    .left-col h1 {
        color: #333;
        font-weight: 600;
        margin-bottom: 30px;
    }

    .house {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        padding: 30px 0;
        border-top: 1px solid #333;
    }

    .house-img {
        flex-basis: 40%;
    }

    .house-img img {
        width: 100%;
        border-radius: 12px;
    }

    .house-info {
        flex-basis: 58%;
        color: #555;
    }

    .house-info h3 {
        font-weight: 600;
        color: #333;
        font-size: 22px;
        margin: 4px 0;
    }

    .house-info i {
        color: #ff5361;
        font-size: 18px;
        margin: 10px 1px;
    }

    .house-price {
        text-align: right;
    }

    .house-price h4 {
        font-size: 20px;
    }

    .right-col {
        flex-basis: 25%;
    }

    .sidebar {
        border: 1px solid #999;
        padding: 20px 30px;
        margin-top: 30px;
    }

    .sidebar h2 {
        font-weight: normal;
        font-weight: 500;
    }

    .sidebar h3 {
        font-weight: 500;
        margin: 20px 0 10px;
    }

    .filter {
        display: flex;
        align-items: center;
        color: #555;
        margin-bottom: 10px;
    }

    .filter p {
        flex: 1;
    }

    .filter input {
        margin-right: 15px;
        cursor: pointer;
    }

    .sidebar-link {
        text-align: right;
        margin: 20px 0;
    }

    .pagination {
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 30px auto;
    }

    .pagination img {
        width: 15px;
        margin: 10px 20px;
    }

    .pagination img:last-child {
        transform: rotate(180deg);
    }

    .pagination span {
        margin: 10px 8px;
        width: 20px;
        height: 40px;
        line-height: 40px;
        text-align: center;
        border-radius: 50%;
        cursor: pointer;
    }

    @media (max-width: 700px) {
        .list-container {
            margin-top: 150px;
        }

        .left-col, .right-col,
        .house-img, .house-info {
            flex-basis: 100%;
        }

        .left-col h1 {
            font-size: 22px;
        }

        .house-info h3 {
            font-size: 18px;
        }
    }
</style>
