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
    /* height: 120px; */
    /* test */

    background-color: white;
}

.container{
    max-width: 1250px;

    margin: 0 auto;
}

nav .container{
    display: flex;
    justify-content: space-between;
    align-items: center;

    padding: 20px 0;
}

nav .container ul{
    display: flex;
    gap: 30px;

    list-style-type: none;
}
</style>