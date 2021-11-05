<template>
        <nav class="nav">
            <a class="logo" href="#landing">S</a>
            <div class="links-container">
                <a class="nav-link" href="#about">About</a>
                <a class="nav-link" href="#portfolio">Portfolio</a>
                <a class="nav-link" href="#contact">Contact</a>  
            </div>
        </nav>
</template>

<style scoped lang="scss">
.nav {
    display: flex;
    padding: 0 12rem 0 12rem;

    .logo {
        font-size: 6rem;
        font-family: $font-primary;
    }
    .links-container {
        align-items: center;
        flex: 1;
        display: flex;
        justify-content: center;

        .nav-link { 
            font-family: $font-secondary;
            font-size: 1.7rem;
            padding: 0 5rem 0 5rem;
        }
    }
}

</style>

