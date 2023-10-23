<template>

  <main>
    <nav>
      <label class="logo">
        <!-- <RouterLink to="/"><img alt="Vue logo" class="logo" src="@/assets/logo.svg"/></RouterLink> -->
        <RouterLink to="/"><p>HairdresserMU</p></RouterLink>
      </label>
      <input type="checkbox" id="check">
      <label for="check" class="checkbtn">
        <i class="fa-regular fa-square-caret-down fa-lg" style="color: #ffffff;"></i>
      </label>
      <ul>
        <li><RouterLink to="/">Home</RouterLink></li>
        <li><RouterLink to="/about">About</RouterLink></li>
        <li><RouterLink to="/services">Services</RouterLink></li>
        <li><RouterLink to="/portfolio">Portfolio</RouterLink></li>
        <li><RouterLink to="/contact">Contact</RouterLink></li>
      </ul>
    </nav>
    
    <RouterView class="routerview"/>

    <footer>
        <!--? Footer Start-->
        <div class="footer-area section-bg">
            <div class="container">
                <div class="footer-top footer-padding">
                    <div class="row  d-flex justify-content-between">
                        <div class="col-xl-3 col-lg-4 col-md-5 col-sm-11">
                            <div class="single-footer-caption mb-50">
                                <!-- logo -->
                                <div class="footer-logo">
                                  <p>HairdresserMU</p>
                                </div>
                                <div class="footer-tittle">
                                    <div class="footer-pera">
                                        <p class="info1">Receive updates and latest news direct from Simply enter.</p>
                                    </div>
                                </div>
                                <div class="footer-number">
                                    <h4>+237 691 259 256</h4>
                                    <p>rosemurielleongolo@gmail.com</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-2 col-lg-2 col-md-3 col-sm-6 col-6">
                            <div class="single-footer-caption mb-50">
                                <div class="footer-tittle">
                                    <h4>Location </h4>
                                    <ul>
                                        <li><a href="#">Yaounde Ecole des Postes</a></li>
                                        <li><a href="#"> Yaounde Essos</a></li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-2 col-lg-2 col-md-3 col-sm-6 col-6">
                            <div class="single-footer-caption mb-50">
                                <div class="footer-tittle">
                                    <h4>Explore</h4>
                                    <ul>
                                        <li><a href="#">Portfolio</a></li>
                                        <li><a href="#">About</a></li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-4 col-lg-4 col-md-6 col-sm-11">
                            <div class="single-footer-caption mb-50">
                                <div class="footer-tittle">
                                    <div class="footer-pera">
                                        <p class="info1">Subscribe now to get daily updates</p>
                                    </div>
                                </div>
                                <!-- Form -->
                                <div class="myform">
                                    <div>
                                        <form>
                                            <input type="email" name="EMAIL" placeholder=" Email Address ">
                                            <div class="form-icon">
                                                <button type="submit" name="submit">Send</button>
                                            </div>
                                            <div class="mt-10 info"></div>
                                        </form>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="footer-bottom">
                    <div class="row d-flex justify-content-between align-items-center">
                        <div class="col-xl-3 col-lg-4">
                            <!-- Footer Social -->
                            <div class="footer-social f-right">
                                <a href="#"><i class="fab fa-twitter"></i></a>
                                <a href="#"><i class="fab fa-facebook-f"></i></a>
                                <a href="#"><i class="fab fa-instagram"></i></a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Footer End-->
    </footer>

    <div id="back-top" @click="scrollToTop">
        <a title="Go to Top" href="#"> <i class="fa-regular fa-hand-pointer"></i></a>
    </div>

  </main>            
</template>

<script setup>
  import { onMounted } from 'vue';
  import { RouterLink, RouterView } from 'vue-router'

  onMounted(()=>{
    const navLinks = document.querySelectorAll('nav ul li a');
    navLinks.forEach(link => {
      link.addEventListener('click', () => {
        if (window.innerWidth < 700) {
          const check = document.querySelector('#check');
          if (check.checked) {
            check.checked = false;
          }else{
            check.checked = true;
          }
        }
      });
    });
  });

  const scrollToTop = () => {
    window.scrollTo({
      top: 0,
      behavior: 'smooth',
    });
  }

</script>

<style scoped>

nav{
  padding:0px 10px;
  background: var(--primary);
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 9999;
}
nav .logo{
  float: left;
  padding: 5px 10px;
  margin-top: 15px;
}
nav .logo p{
  color: #fff;
  font-size: 35px;
  font-weight: 700;
  margin: 0 !important;
}
nav .logo p:hover{
  color: var(--secondary);
}

nav ul{
  float: right;
  margin-right: 20px;
  margin-bottom: 0px;
}
nav ul li{
  display: inline-block;
  line-height: 80px;
  position:relative;
  z-index:1;
  margin: 0 5px;
}
nav ul li a{
  color:#fff;
  font-weight:600;
  padding:5px 10px;
  display:block;
  font-size:20px;
  -webkit-transition:.3s;
  -moz-transition:.3s;
  -o-transition:.3s;
  transition:.3s;
  text-transform:capitalize;
  position:relative;
}

nav ul li a::before{
  position:absolute;
  content:"";
  width:14px;
  height:1px;
  background:var(--secondary);
  left:25px;
  bottom:33px;
  transform:rotate(-46deg);
  opacity:0;
  visibility:hidden;
  -webkit-transition:.4s;
  -moz-transition:.4s;
  -o-transition:.4s;
  transition:.4s;
}
nav ul li a::after{
  position:absolute;
  content:"";
  width:14px;
  height:1px;
  background:var(--secondary);
  left:57px;
  top:37px;
  transform:rotate(-46deg);
  opacity:0;
  visibility:hidden;
  -webkit-transition:.4s;
  -moz-transition:.4s;
  -o-transition:.4s;
  transition:.4s;
}
nav ul li:hover a{
  color: var(--secondary);
}
nav ul li:hover a::before {
  opacity:1;
  visibility:visible;
}
nav ul li:hover a::after {
  opacity:1;
  visibility:visible;
}
nav ul li a.router-link-exact-active{
  color:var(--secondary);
}
nav ul li a.router-link-exact-active::before{
  opacity:1;
  visibility:visible;
}

nav ul li a.router-link-exact-active::after{
  opacity:1;
  visibility:visible;
}

.checkbtn{
  font-size: 20px;
  color: #fff;
  line-height: 60px;
  margin-right: 30px;
  float: right;
  cursor: pointer;
  display: none;
}

#check{
  display: none;
}

.routerview{
  margin-top: 90px;
  width: 100%;
}
.footer-area{
  margin-top: 20px;
  background-image: url(../src/assets/footer_bg.png);
}
.footer-area .footer-logo p{
  color: var(--primary);
  font-size: 35px;
  font-weight: 700;
  margin: 0 !important;
}
.footer-area .footer-logo p:hover{
  color: var(--secondary);
}
.footer-area .footer-top{
  border-bottom:1px solid var(--secondary)
}
.footer-area .footer-top .single-footer-caption .footer-logo{
  margin-bottom:20px;
}
.footer-area .footer-top .single-footer-caption .footer-pera .info1{
  line-height:1.8;
  margin-bottom:15px;
  color:var(--secondary);
  padding-right:0px;
}
.footer-area .footer-top .single-footer-caption .footer-number h4{
  color:var(--primary);
  font-size:30px;
  font-weight:500;
  text-transform:capitalize;
}
.footer-area .footer-top .single-footer-caption .footer-number p{
  color:#7c7c7c;
}
.footer-area .footer-top .single-footer-caption .footer-tittle h4{
  color:var(--secondary);
  font-family:"Poppins",sans-serif;
  font-size:14px;
  margin-top: 20px;
  margin-bottom:18px;
  font-weight:600;
  text-transform:uppercase;
}
.footer-area .footer-top .single-footer-caption .footer-tittle ul li{
  color:#7c7c7c;
  margin-bottom:5px;
}
.footer-area .footer-top .single-footer-caption .footer-tittle ul li a{
  color:#7c7c7c;
  font-weight:300;
  font-size:15px
}
.footer-area .footer-top .single-footer-caption .footer-tittle ul li a:hover{
  color: var(--primary);
  padding-left:5px
}
.footer-area .footer-top .single-footer-caption .myform{
  margin-bottom:10px
}
.footer-area .footer-top .single-footer-caption .myform form{
  position:relative;
}
.footer-area .footer-top .single-footer-caption .myform form input:focus{
  border: 1px solid var(--primary);
}
.footer-area .footer-top .single-footer-caption .myform form input{
  width:100%;
  height:43px;
  padding:10px 20px;
  border:0;
  background:#101720;
  color:#fff;
  outline: 0;
}
.footer-area .footer-top .single-footer-caption .myform form input::placeholder{
  color:#7c7c7c;
  font-weight:300;
  font-size:14px
}
.footer-area .footer-top .single-footer-caption .myform form .form-icon button{
  position:absolute;
  top:1px;
  right:1px;
  background:none;
  border:0;
  cursor:pointer;
  padding: 13px 18px;
  background:#0a0f17;
  line-height:1;
  color:var(--primary);
  font-size:14px;
  font-weight:300
}
.footer-area .footer-top .single-footer-caption .footer-cap{
  margin-bottom:30px
}
.footer-area .footer-top .single-footer-caption .footer-cap span{
  color:var(--primary);
  font-size:16px;
  font-weight:300;
  margin-bottom:10px;
  display:block
}
.footer-area .footer-top .single-footer-caption .footer-cap p{
  color:#7c7c7c;
  font-size:16px
}
.footer-area .footer-bottom{
  padding-bottom:50px;
  padding-top:30px
}


.footer-area .footer-social span{
  color:#fff;
  position:relative;
  margin-right:57px
}
.footer-area .footer-social span::before{
  position:absolute;
  content:"";
  width:43px;
  height:2px;
  background:#3b3647;
  top:50%;
  transform:translateY(-50%);
  right:-56px
}
.footer-area .footer-social a{
  color:#7c7c7c;
  font-size:14px;
  padding-left:25px
}
.footer-area .footer-social a i{
  -webkit-transition:.4s;
  -moz-transition:.4s;
  -o-transition:.4s;
  transition:.4s;
  transform:rotateY(0deg);
}
.footer-area .footer-social a:hover{
  color:#fff
}
.footer-area .footer-social a:hover i{
  transform:rotateY(180deg)
}
#back-top{
  background:var(--primary);
  height:50px;
  width:50px;
  right:31px;
  bottom:18px;
  position:fixed;
  color:#fff;
  font-size:20px;
  text-align:center;
  border-radius:50%;
  line-height:48px;
  border:2px solid transparent;
  box-shadow:0 0 10px 3px rgba(108,98,98,0.2)}

@media only screen and (min-width: 691px) and (max-width: 850px){
  nav .logo{
  padding: 2px 7px;
  margin-top: 13px;
}
nav .logo p{
  font-size: 25px;
}

nav ul{
  margin-right: 10px;
}
nav ul li{
  line-height: 60px;
}
nav ul li a{
  padding:2px 7px;
  font-size:18px;
}

nav ul li a::before{
  left:15px;
  bottom:23px;
}
nav ul li a::after{
  left:37px;
  top:27px;
}
.routerview{
  margin-top: 64px;
}
.footer-area .footer-social{
  float:left;
  padding-top:10px;
}
}
@media (max-width: 691px){
  nav{
    padding:0px;
  }
  nav .logo{
    padding: 2px 7px;
    margin-top: 10px;
  }
  nav .logo p{
    font-size: 25px;
    font-weight: 600;
  }
  nav ul{
    display: fixed;
    width: 100%;
    height: 0;
    margin-right: 0px;
    background-color: var(--secondary);
    text-align: center;
    top: 64px;
    left: 0;
    padding-left: 0;
    z-index: 9999;
    transition: height 0.3s ease;
    overflow: hidden;
  }
  nav ul li{
    display: block;
    margin: 50px 0;
    line-height: 30px;
    width: 100%;
  }
  nav ul li a{
    font-size: 20px;
  }
  nav ul li a:hover{
    color: var(--primary);
  }
  nav ul li a.router-link-exact-active{
    color:var(--primary);
  }
  .checkbtn{
    display: block;
  }
  #check:checked ~ ul{
    height: 100vh;
  }
  .routerview{
    margin-top: 60px;
  }
}
  
</style>
