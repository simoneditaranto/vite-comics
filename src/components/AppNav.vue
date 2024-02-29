<script>

export default {
    name: 'AppNav'
}

</script>

<template>
    
    <nav>

        <div class="container">
            
            <img src="/img/dc-logo.png" alt="dc logo">

            <ul>

                <li>link</li>
                <li>link</li>
                <li>link</li>
                <li>link</li>
                <li>link</li>
                <li>link</li>
                <li>link</li>
                <li>link</li>
                <li>link</li>
                <li>link</li>

            </ul>

        </div>
        
    </nav>

</template>

<style>

nav{
    background-color: white;
}

.container{
    /* padding: 20px 0; */
    margin: 0 auto;

    max-width: 1250px;
}

nav .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
}

nav .container img{
    margin-top: 50px;
}

nav .container ul{
    display: flex;
    gap: 30px;

    list-style-type: none;
}
</style>