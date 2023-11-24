<nav>
    <a href="/">Главная</a>
    <a href="/logs">Логи</a>
    <a href="/stat">Статистика</a>
</nav>


<style>
    nav {
        background: rgb(2,0,36);
        background: linear-gradient(90deg, rgba(2,0,36,1) 0%, rgba(79,79,194,1) 64%, rgba(0,212,255,1) 100%);
        margin: 0;
        padding: 1em;
        display: flex;
    }

    a {
        padding: 1em;
        text-decoration: none;
    }
    a:after {
        color:black;
    }
</style>

<slot />