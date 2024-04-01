<template>
    <header class="header">
        <div class="header__contenedor">
            <div class="header__barra">
                <a href="">
                    <img src="../assets/Logo2-removebg-preview.png" alt="imagen logo" class="header__logo">
                </a>
                <nav class="navegacion">
                    <a href="index.html" class="navegacion__enlace">Inicio</a>
                    <a href="nosotros.html" class="navegacion__enlace">Nosotros</a>
                    <a href="blog.html" class="navegacion__enlace">Blog</a>
                    <a href="tienda.html" class="navegacion__enlace">Tienda</a>
                </nav>
            </div><!--.header-barra-->
            
            <div class="modelo">
                <h1 class="modelo__nombre">Apple iPhone 15 5G 128GB</h1>
                <p class="modelo__description">Sistema Operativo: iOS 17 Procesador:A16 Bionic - CPU 6 Core - GPU 5 Core - Neuronal Engine 16 Core  Memoria RAM: 6 GB  Capacidad Almacenamiento: 128 GB  Pantalla: Super Retina XDR OLED  Tamaño de Pantalla: 6.1 Pulgadas </p>
                <p class="modelo__precio">$912.000</p>
                <a href="producto.html" class="modelo__enlace">Ver Detalles</a>
            </div>
            <img src="../assets/iPhone_15_-_Black_-_2-removebg-preview.png" alt="imagen header guitarra" class="header__guitarra">
        </div>
    </header>   
</template>


<style>

.header {
    background-image: linear-gradient(to right, rgb(0 0 0 /.7), rgb(0 0 0 /.7)), url(/src/assets/header2.png);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: 50%;
    padding: 5rem 0;
    position: relative;
    /* height: 100vh; */
}


.header__guitarra {
    display: none;
}



@media (min-width:992px) {
    .header__guitarra {
        display: block;
        position: absolute;
        right: 0;
        bottom: 0;
        animation: 1s ease-in-out 0s 1 mostrarImagen;
    }    

}

@keyframes mostrarImagen {
    0% {
        opacity: 0;
        transform: translateX(-10rem);
        
    }
    50% {
        opacity: 0;
        

    }
    100% {
        opacity: 1;
        transform: translateX(0rem);
    }
}

.header__barra {
    display: flex;
    flex-direction: column;
    align-items: center;
}

@media (min-width:768px) {
    .header__barra{
        flex-direction: row;
        justify-content: space-between;
    }
}

.header__logo {
    width: 30rem;
}

.navegacion {    
    display: flex;
    gap: 2rem;
    margin-top: 5rem;
    position: relative;
    z-index: 1;
}

@media (min-width:768px) {
    .navegacion {
        margin-top: 0;        
    }
}



.navegacion__enlace{
    border-radius: 1rem;
    color: var(--blanco);
    text-decoration: none;
    text-transform: uppercase;
    padding: .5rem;
    font-size: 1.4rem;
    font-weight: 700;
    transition-property: background-color;
    transition-duration: .3s; 
}

.navegacion__enlace:hover {
    background-color: var(--primary);
}

.modelo {
    color: var(--blanco);
    margin-top: 5rem;
    text-align: center;


}

@media (min-width:768px) {
    .modelo {
        text-align: left;
        width: 50%;
    }
}


.modelo__nombre {    
    font-size: 6rem;
    
}

.modelo__precio {
    color: var(--primary);
    font-size: 6rem;
    font-weight: 900;
    line-height: 0;
    
}

.modelo__enlace {
    border-radius: 2rem;
    border: 2px solid var(--primary);
    color: var(--blanco);
    margin-top: 2rem;
    text-decoration: none;
    padding: 1rem 5rem;
    text-transform: uppercase;
    font-weight: 700;
    font-size: 1.4rem;
    transition-property: background-color;
    transition-duration: .3s;
    
}

.modelo__enlace:hover {        
    background-color: var(--primary);
}

</style>
