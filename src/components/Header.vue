<template>
    <div class="Header">
        <h1>Team View</h1>
        <div class="Nav">
            <ul>
                <li><router-link :to="{ name: 'Home'}">Home</router-link></li>
                <li><router-link to="/About">About</router-link></li>
            </ul>
        </div>
        <router-view/>
    </div>
</template>

<script>
export default {

}
</script>

<style>

ul {
    list-style-type: none;
    text-align: center;
    margin: 0;
    }

li {
    display: inline-block;
    margin: 0 10px;
}

.Nav {
    background: #444;
    padding: 14px 0;
    margin-bottom: 40px;
}

.Nav a {
    color: #fff;
    text-decoration: none;
    padding: 6px 8px;
    border-radius: 10px;
}

</style>