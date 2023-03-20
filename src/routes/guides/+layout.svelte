<nav>
    <div class="links">
        <a href="/">Home</a>
        <a href="/about">About</a>
        <a href="/guides">Guides</a>
    </div>
</nav>

<main>
    <slot></slot>
</main>

<style>
    nav {
        display: flex;
        justify-content: center;
        background-color: rgb(45, 21, 76);
        padding: 10px;
    }
    main {
        max-width: 960px;
        margin: 20px auto;
    }
    .links {
        margin-left: auto;
    }
    a {
        margin-left: 10px;
    }
</style>