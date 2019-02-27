<template>
    <div class="header-container">
        <h1>DevCat</h1>
        <p>Explore the &lt;front&gt;&#123;end&#125; world</p>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.header-container {
    text-align: center;
}

.header-container h1 {
    font-family: 'Signika', sans-serif;
    font-size: 3.5rem;
    letter-spacing: 2px;
}

.header-container p {
    font-family: 'Open Sans', sans-serif;
    font-size: 1.2rem;
    margin-top: -15px;
    margin-bottom: 10%;
    opacity: .8;
    letter-spacing: 3px;
}

@media screen and (max-width: 750px) {
    .header-container h1 {
        font-size: 2.5rem;
    }

    .header-container p {
        font-size: .9rem;
    }
}
</style>
