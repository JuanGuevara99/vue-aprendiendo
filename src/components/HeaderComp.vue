<template>
<nav class="navbar navbar-expand-lg bg-body-tertiary fixed-top">
    <div class="container-fluid">
        <router-link to="/" class="navbar-brand">
            <img src='../images/logo2.png' alt="" class="navbar_logo">
        </router-link>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
            <ul class="navbar-nav me-auto">
                <li class="nav-item">
                    <router-link to="/" class="nav-link active" aria-current="page">Inicio</router-link>
                </li>
                <li class="nav-item">
                    <router-link to="/store" class="nav-link" href="#">Tienda</router-link>
                </li>
                <li class="nav-item dropdown">
                    <a class="nav-link dropdown-toggle" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                        Nosotros
                    </a>
                    <ul class="dropdown-menu">
                        <li>
                            <router-link class="dropdown-item" to="/about">Unirse</router-link>
                        </li>
                        <li><a class="dropdown-item" href="/about#about">¿Quiénes somos?</a></li>
                        <li><a class="dropdown-item" href="/about#services">Sevicios</a></li>
                        <li><a class="dropdown-item" href="/about#contact">Contacto</a></li>
                    </ul>
                </li>
            </ul>
            <ul class="navbar-nav ms-auto">
                <li class="nav-item d-none d-lg-block">
                    <a class="nav-link" href="#" @click="toggleSearchForm"><i class="ri-search-line"></i></a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                        <i class="ri-heart-line"></i>
                        <span class="badge">1</span>
                        <span class="d-lg-none"> Mis favoritos</span>
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                        <i class="ri-shopping-cart-line"></i>
                        <span class="badge">1</span>
                        <span class="d-lg-none"> Mi carrito</span>
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#"><img src='../images/user-icon.png' alt="" class="user-icon"><span class="d-lg-none"> Iniciar sesión</span></a>
                </li>
            </ul>
            <div v-if="showSearchForm" class="search-form-lg d-none d-lg-block">
                <form class="d-flex" role="search">
                    <input class="form-control me-2" type="search" placeholder="Buscar" aria-label="Buscar">
                    <button class="btn btn-outline-success" type="submit"><i class="ri-search-line"></i></button>
                </form>
            </div>
            <div class="d-lg-none ms-auto">
                <form class="d-flex" role="search">
                    <input class="form-control me-2" type="search" placeholder="Buscar" aria-label="Buscar">
                    <button class="btn btn-outline-success" type="submit"><i class="ri-search-line"></i></button>
                </form>
            </div>
        </div>
    </div>
</nav>
</template>

<script>
export default {
    data() {
        return {
            showSearchForm: false,
        };
    },
    methods: {
        toggleSearchForm() {
            this.showSearchForm = !this.showSearchForm;
        },
    },
};
</script>

<style scoped>
@import url('../assets/css/style.css');

.navbar_logo {
    width: 150px;
    height: auto;
}

.nav-link {
    display: flex;
    align-items: center;
    position: relative;
}

.user-icon {
    width: 35px;
    height: auto;
    margin-right: 8px;
}

.badge {
    position: absolute;
    top: 5px;
    right: 5px;
    width: 18px;
    height: 18px;
    background: var(--primary-color);
    color: var(--text-color);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.7rem;
    font-weight: 600;
    z-index: 10;
}

.nav-link i {
    font-size: 1.5em;
    margin-left: 1px;
    margin-right: 8px
}

.search-form-lg {
    position: absolute;
    top: 60px;
    right: 180px;
    background: var(--text-color);
    padding: 10px;
    border: 1px solid var(--primary-color);
    border-radius: 5px;
    z-index: 1000;
}

.search-form-lg .form-control {
    width: 200px;
}

@media (min-width: 992px) {
    .search-form-lg {
        display: none;
    }
}

@media (max-width: 991px) {
    .nav-link .badge {
        position: relative;
        top: -5px;
        right: 14px; 
    }
}
</style>
