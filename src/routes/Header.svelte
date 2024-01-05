<script>
    let menuItems = [
        { label: 'Home', link: '/' },
        { label: 'About', link: '/about' },
        { label: 'Contact', link: '/contact' },
    ];
</script>

<style>
    .menu-bar {
        background-color: transparent;
        display: flex;
        justify-content: space-between;
        padding: 1rem;
    }

    .menu-item {
        margin-right: 1rem;
        color: rgb(134, 11, 11);
        text-decoration: none;
        cursor: pointer;
    }
</style>

<div class="menu-bar">
    {#each menuItems as item}
        <a class="menu-item" href={item.link}>{item.label}</a>
    {/each}
</div>
