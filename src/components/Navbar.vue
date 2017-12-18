<template>

    <div class="root">
        <nav class="navbar navbar-default">
            <ul class="nav navbar-nav">
                <li v-for="list in navbarList"><a href="#">{{ list }}</a></li>
            </ul>
        </nav>
    </div>



</template>



<script>
    export default {
        props:['navbarList']
    }


</script>




<style>

</style>