<template>
    <div>
        <h3>Edit the User {{ $route.params.id }}</h3>
        <p>Locale: {{ $route.query.locale }}</p>
        <p>Analytics: {{ $route.query.q }}</p>
        <div style="height:700px" ></div>
        <p id="data"></p>


    </div>
</template>
<script>
    export default {
        beforeRouteLeave(to,from,next){
            if(confirm("are you sure?"))
            {
                next();
            }
            else{
                next(false);
            }

        }
    }
</script>