<script>
    import Router, {location} from "svelte-spa-router";

    import NotFound from "./Routers/notFound.svelte";
    import OnlinePackages from "./Routers/onlinePackages.svelte";
    import PopularPlaces from "./Routers/popularPlaces.svelte";
    import TravelOutside from "./Routers/travelOutside.svelte";

    import Header from "./components/Header.svelte";
    import Footer from "./components/Foot.svelte";

    let routes = {
        "/": PopularPlaces,
        "/travel": TravelOutside,
        "/packages": OnlinePackages,
        "*": NotFound,
    };

    $: $location;
</script>

<main>
    <Header local={$location}>
        <nav class="nav-links">
            <img src="/images/logo.png" alt="logo" class="logo">

            <ul>
                <li>
                    <a href="/#/">Home</a>
                </li>

                <li>
                    <a href="/#/travel">Recommended Places</a>
                </li>

                <li>
                    <a href="/#/packages">Hot House in moment</a>
                </li>
            </ul>

            <button class="register-btn">Register Now</button>
        </nav>
    </Header>

    <div class="container">
        <Router {routes} />

        <Footer />
    </div>
</main>

<style>
    .nav-links {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px 7%;
    }

    .register-btn {
        display: inline;
        border: none;
        background: #fff;
        color: #000;
        padding: 8px 20px;
        font-size: 14px;
        border-radius: 20px;
        cursor: pointer;
    }

    ul {
        display: flex;
        list-style: none;
        gap: 20px;
    }

    li a {
        color: #fff;
    }

    .logo {
        width: 140px;
        cursor: pointer;
    }

    @media (max-width: 800px) {
        .nav-links {
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
        }
    }
</style>