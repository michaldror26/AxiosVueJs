<template>
    <div id="nav">
        <ul class="nav nav-pills">
            <router-link to="/" tag="li" active-class="active" exact><a class="kk">Home</a></router-link>
            &nbsp&nbsp&nbsp
            <router-link to="/user" tag="li" active-class="active"><a>User</a></router-link>
            &nbsp&nbsp&nbsp
            <router-link to="/app2" tag="li" active-class="active"><a>App2</a></router-link>
            &nbsp&nbsp&nbsp
        </ul>
    </div>
</template>
<style lang="scss">
    #nav {
        padding: 30px;
        a {
            font-weight: bold;
            color: #2c3e50;
            &.router-link-exact-active {
                color: #42b983;
            }
        }

    }

</style>