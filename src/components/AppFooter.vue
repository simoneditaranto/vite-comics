<script>

export default{
    name: 'AppFooter'
}

</script>

<template>

    <footer>

        <div class="container">
            
            <div class="links">

                <div class="link-list">
                    <h3>DC COMICS</h3>
                    <ul>

                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>

                    </ul>
                </div>

                <div class="link-list">
                    <h3>DC COMICS</h3>
                    <ul>

                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>

                    </ul>
                </div>

            </div>

            
                <img src="/img/dc-logo-bg.png" alt="">
           
            
            
        </div>
        
    </footer>

</template>

<style>

footer{
    background-image: url('/img/footer-bg.jpg');
    background-size: cover;
}

footer .container{
        display: flex;
        justify-content: space-between;
        align-items: flex-start;

        color: white;
}

footer .container .links {
    display: flex;
    gap: 55px;

    padding: 45px 0 0;
}


footer .container h3{
    margin-bottom: 20px;
}

footer .container ul{
    list-style-type: none;
}

/* img{
    transform: translateY(-25%);
} */

</style>