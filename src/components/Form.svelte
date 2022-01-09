<div class="search-bar">
    <form>
        <div class="location-input">
            <label for="location">Location</label>

            <input type="text" id="location" placeholder="Where are you going?">
        </div>

        <div>
            <label for="checkin">Check in</label>

            <input type="date" id="checkin">
        </div>

        <div>
            <label for="checkout">Check out</label>

            <input type="date" id="checkout">
        </div>

        <div>
            <label for="guest">Guest</label>

            <input type="text" id="guest" placeholder="Add Guest">
        </div>

        <button type="submit">
            <img src="/images/search.png" alt="button">
        </button>
    </form>
</div>

<style>
    .search-bar {
        background: #fff;
        width: 70%;
        margin: 30px auto;
        padding: 6px 10px 6px 30px;
        border-radius: 50px;
    }

    .search-bar form {
        display: flex;
        align-items: center;
        flex-wrap: wrap;
    }

    .search-bar form input {
        display: block;
        border: 0;
        outline: none;
        background: transparent;
    }

    .search-bar form button {
        background: #ff5361;
        width: 55px;
        height: 55px;
        border-radius: 50%;
        border: none;
        outline: none;
        cursor: pointer;
    }

    .search-bar form button img {
        width: 15px;
        margin-top: 7px;
    }

    .location-input {
        flex: 1;
    }

    .search-bar form label {
        font-weight: 600;
        
    }
</style>