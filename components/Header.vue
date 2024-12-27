<template>
    <nav class="navbar navbar-expand-lg bg-success">
        <div class="container">
            <img src="/assets/img/LOGO SMKN 4.png" alt="LOGO" width="100px" height="100px">
            <a class="navbar-brand" href="#">SMKN 4 TASIKMALAYA</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                        <li class="nav-item">
                        <NuxtLink class="nav-link" :class="{ active: route.name == 'fasilitas' }" to="/fasilitas">fasilitas</NuxtLink>
                    </li>
                    <li class="nav-item">
                        <NuxtLink class="nav-link" :class="{ active: route.name == 'jurusan' }" to="/jurusan">jurusan</NuxtLink>
                    </li>
                    <li class="nav-item">
                        <NuxtLink class="nav-link" :class="{ active: route.name == 'profil sekolah' }" to="/profil sekolah">profil sekolah</NuxtLink>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script setup>
const route = useRoute()

console.log(route.name)
</script>