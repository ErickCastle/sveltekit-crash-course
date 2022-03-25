<script>
    import Title from "$lib/title.svelte";
    import "../../styles/global.css"
</script>

<header>
    <nav>
        <Title title="Castle Gaming Guides"/>
        <div class="links">
            <a href="/">Home</a>
            <a href="/about">About Us</a>
            <a href="/guides">Guides</a>
        </div>
    </nav>
</header>

<main>
    <!-- Page Content -->
    <slot></slot>
</main>

<footer>
    <p>Copyright 2022 Castle Gaming Guides</p>
</footer>

<style>
    header {
        text-align: center;
        background: rgba(0, 0, 0, 0.1);
        justify-content: center;
    }
    main {
        max-width: 960px;
        margin: 20px auto;
    }
    footer {
        text-align: center;
    }
    .links {
        margin-left: auto;
    }
    a {
        margin-left: 10px;
    }
    nav {
        display: flex;
        align-items: center;
        max-width: 960px;
        margin: 0 auto;
    }
</style>