<template>
    <div id="nav">
        <img class="logo" alt="Boardgame logo" src="../assets/logo_boardgame.png"><br/>
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
            <div class="collapse navbar-collapse justify-content-md-center" id="navbarNavDropdown">
                <ul class="navbar-nav">
                    <li class="nav-item active">
                        <router-link class="nav-link" to="/">Accueil</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="nav-link" to="/players">Joueurs</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="nav-link" to="/games">Jeux</router-link>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuAdmin" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            Admin
                        </a>
                        <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuAdmin">
                            <router-link class="dropdown-item" to="/createPlay">Ajouter une partie</router-link>
                            <router-link class="dropdown-item" to="/createPlayer">Ajouter un joueur</router-link>
                            <router-link class="dropdown-item" to="/createGame">Ajouter un jeu</router-link>
                        </div>
                    </li>
                </ul>
            </div>
        </nav>
    </div>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped>
    .logo {
        height: 200px;
    }

    #nav a {
         font-weight: bold;
         color: rgba(0,0,0,.5);
         text-decoration: none;
     }

    #nav a.router-link-exact-active {
        color: rgba(0,0,0,.9);
    }

</style>