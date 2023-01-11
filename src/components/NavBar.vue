<template>
    <nav class="navbar navbar-expand-lg">
        <div class="container-fluid justify-content-between">
            <a class="navbar-brand" href="#">Hoodies</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse justify-content-center" id="navbarNav">
                <ul class="list navbar-nav gap-4">
                    <li class="nav-item">
                        <router-link class="list-items" to="/">Home</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="list-items" to="/product">Products</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="list-items" to="/about">About</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="list-items" to="/contact">Contact</router-link>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>
<script>
export default {
};
</script>

<style>
.list{
    text-decoration: none;
}
.navbar {
    background-color: #7e0328;
}
.list-items {
    color: grey;
    text-decoration: none;
}
.list-items:hover{
    color: #7e0328;
    background-color: grey;
    border-radius: 4px;
}
</style>
