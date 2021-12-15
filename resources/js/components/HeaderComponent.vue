<template>
    <header>
        <section class="contact pt-2 pb-2">
            <div class="container">
                <div class="row">
                    <div class="col-md-6 d-flex">
                        <img src="image/Path.png" alt="">
                        <p class="text-white ms-2"> +880 1254 698 624</p>
                    </div>

                    <div class="col-md-6 socialFooter">
                        <div class="socialIcon">
                            <a href="#"><i class="fab fa-facebook-f"></i></a>
                            <a href="#"><i class="fab fa-twitter"></i></a>
                            <a href="#"><i class="fab fa-linkedin-in"></i></a>
                            <a href="#"><i class="fab fa-instagram"></i></a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <nav class="navbar navbar-expand-lg navbar-light ">
            <div class="container">
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
                    aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <a href="#">
                    <img src="image/kxLogo.svg" alt="">
                </a>
                <div class="navbar-toggler">
                    <a href="#" class=" navLogin">
                        <i class="far fa-user "></i> login
                    </a>
                </div>

                <div class="collapse navbar-collapse ms-5" id="navbarSupportedContent">
                    <ul class="navbar-nav m-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="page/trackingPage.html">Tracking</a>
                        </li>

                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button"
                                data-bs-toggle="dropdown" aria-expanded="false">
                                Our Service
                            </a>
                            <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                                <li><a class="dropdown-item" href="#">Action</a></li>
                                <li><a class="dropdown-item" href="#">Another action</a></li>
                                <li>
                                    <hr class="dropdown-divider">
                                </li>
                                <li><a class="dropdown-item" href="#">Something else here</a></li>
                            </ul>
                        </li>

                        <li class="nav-item">
                            <a class="nav-link" href="page/pricingTable.html">Pricing</a>
                        </li>

                        <li class="nav-item">
                            <a class="nav-link" href="#">Coverage Area</a>
                        </li>

                        <li class="nav-item">
                            <a class="nav-link" href="page/faq.html">FAQ</a>
                        </li>

                    </ul>
                    <form class="d-flex">

                        <button class="btn heroButton" type="button" id="inputGroupFileAddon04">Join With KX</button>

                    </form>
                    <div class="loginInfo">
                        <a class="nav-link" href="#"> <i class="far fa-user"></i> login</a>
                    </div>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
    export default {
        mounted() {
            console.log('Component mounted.')
        }
    }
</script>
