<script>
    export let local;

    import Form from "./Form.svelte";
</script>

{#if local === "/"}
    <header class="header">
        <slot />

        <div class="container">
            <h1>Find Your Next Stay</h1>
            <Form />
        </div>
    </header>
{:else}
    <header class="out">
        <slot />
    </header>
{/if}

<style>
    .header {
        min-height: 100vh;
        width: 100%;
        background-image: linear-gradient(
                rgba(0, 0, 0, 0.3),
                rgba(0, 0, 0, 0.3)
            ),
            url("/images/banner.png");
        background-size: cover;
        background-position: center;
    }

    .out {
        background: #000;
    }

    h1 {
        font-size: 4vw;
        font-weight: 500;
        color: #fff;
        text-align: center;
        padding-top: 15%;
    }
</style>
