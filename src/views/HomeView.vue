<template>
  <main>
    <div class="slider-area">
      <div class="slider-active">
        <!-- Single Slider -->
        <div class="single-slider slider-height d-flex align-items-center">
          <div class="container">
            <div class="row">
              <div class="col-xl-8 col-lg-9 col-md-11 col-sm-10">
                <div class="hero__caption">
                  <span>with Murielle MBOMO</span>
                  <h1>Our Hair Style make your look elegance</h1>
                </div>
                <!-- stroke Text -->
                <div class="stock-text">
                  <h2>Get More confident</h2>
                  <h2>Get More confident</h2>
                </div>
              </div>
            </div>
          </div>          
        </div>
      </div>
      <!-- Arrow -->
      <div class="thumb-content-box" @click="showPopup">
        <div class="thumb-content">
          <h3>make an appointment now</h3>
          <i class="fa-regular fa-circle-right fa-beat-fade" style="color: #000000;"></i>
        </div>
      </div>
      <AppointmentCard v-if="show" :showAppointment="show" @showAppointmentPopup="showPopup"/>
    </div>
    <!-- slider Area End-->
    <!--? About Area Start -->
    <section class="about-area">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-lg-6 col-md-11">
            <!-- about-img -->
            <div class="about-img">
              <img src="@/assets/MGIJ1795.png" alt="">
            </div>
          </div>
          <div class="col-lg-6 col-md-12">
            <div class="about-caption">
              <!-- Section Tittle -->
              <div class="section-title mb-25">
                <span>About Our company</span>
                <h2>10 Years Of Experience In Hair cut!</h2>
              </div>
              <p class="mb-30 pera-bottom">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Commodi, dolorem in consequuntur cumque excepturi officiis explicabo eveniet magni ullam ut eos a natus repellendus, inventore ipsa aut culpa laborum! Unde.</p>
              <p class="pera-top mb-50">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ea voluptatem quae vero eaque eligendi corrupti.</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- About-2 Area End -->
    <!--? Services Area Start -->
    <section class="service-area pb-170">
      <div class="container">
        <!-- Section Tittle -->
        <div class="row d-flex justify-content-center">
            <div class="col-xl-7 col-lg-8 col-md-11 col-sm-11">
                <div class="section-title text-center mb-90">
                    <span>Professional Services</span>
                    <h2>Our Best services that  we offering to you</h2>
                </div>
            </div>
        </div>
        <!-- Section caption -->
        <div class="row">
            <div class="col-xl-4 col-lg-4 col-md-6">
                <div class="services-caption text-center mb-30">
                    <div class="service-icon">
                      <img src="@/assets/MHLZ0467.png" alt="...">
                    </div> 
                    <div class="service-cap">
                        <h4>Stylish Hair Cut</h4>
                        <p>Sorem spsum dolor sit amsectetur adipisclit, seddo eiusmod tempor incididunt ut laborea.</p>
                    </div>
                </div>
            </div>
            <div class="col-xl-4 col-lg-4 col-md-6">
                <div class="services-caption active text-center mb-30">
                    <div class="service-icon">
                      <img src="@/assets/TDTG9998.png" alt="...">
                    </div> 
                    <div class="service-cap">
                        <h4>Body Massege</h4>
                        <p>Sorem spsum dolor sit amsectetur adipisclit, seddo eiusmod tempor incididunt ut laborea.</p>
                    </div>
                </div>
            </div> 
            <div class="col-xl-4 col-lg-4 col-md-6">
                <div class="services-caption text-center mb-30">
                    <div class="service-icon">
                      <img src="@/assets/TMZX0632.png" alt="...">
                    </div> 
                    <div class="service-cap">
                        <h4>Breard Style</h4>
                        <p>Sorem spsum dolor sit amsectetur adipisclit, seddo eiusmod tempor incididunt ut laborea.</p>
                    </div>
                </div>
            </div>
            <div class="col-xl-4 col-lg-4 col-md-6">
                <div class="services-caption text-center mb-30">
                    <div class="service-icon">
                      <img src="@/assets/PBKK5683.png" alt="...">
                    </div> 
                    <div class="service-cap">
                        <h4>Breard Style</h4>
                        <p>Sorem spsum dolor sit amsectetur adipisclit, seddo eiusmod tempor incididunt ut laborea.</p>
                    </div>
                </div>
            </div>
        </div>
      </div>
    </section>
    <!-- Services Area End -->
    <!--? Team Start -->
    <div class="team-area pb-180">
      <div class="container">
        <!-- Section Tittle -->
        <div class="row justify-content-center">
            <div class="col-xl-8 col-lg-8 col-md-11 col-sm-11">
                <div class="section-title text-center mb-100">
                    <span>Professional Teams</span>
                    <h2>Our hairdresser experts for you</h2>
                </div>
            </div>
        </div>
      
        <!-- single Tem -->
        <div id="carouselExampleCaptions" class="carousel slide">
          <div class="carousel-indicators">
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
          </div>
          <div class="carousel-inner">
            <div class="carousel-item active">
              <img src="@/assets/HQWV9777.png" class="d-block w-100 team-img" alt="...">
              <div class="carousel-caption d-md-block team-caption text-center">
                <h5>First slide label</h5>
                <p>Some representative placeholder.</p>
              </div>
            </div>
            <div class="carousel-item">
              <img src="@/assets/LPRA4797.png" class="d-block w-100" alt="...">
              <div class="carousel-caption team-caption d-md-block text-center">
                <h5>Second slide label</h5>
                <p>Some representative placeholder.</p>
              </div>
            </div>
            <div class="carousel-item">
              <img src="@/assets/KQDD8499.png" class="d-block w-100" alt="...">
              <div class="carousel-caption team-caption d-md-block text-center">
                <h5>Third slide label</h5>
                <p>Some representative placeholder.</p>
              </div>
            </div>
          </div>
          <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
          </button>
          <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
          </button>
        </div>

      </div>
        
    </div>
    <!-- Team End -->
    <!-- Best Pricing Area Start -->
    <div class="best-pricing position-relative">
        <div class="container">
            <div class="row justify-content-end">
                <div class="col-xl-12 col-lg-12">
                    <div class="section-title text-center mb-50">
                        <span>Our Best Pricing</span>
                        <h2>We provide best price<br> in the city!</h2>
                    </div>
                    <!-- Pricing  -->
                    <div class="row">
                        <!-- pricing list -->
                        <div class="col-lg-6 col-md-6 col-sm-6">
                            <div class="pricing-list">
                                <ul>
                                    <li>Rasta. . . . . . . . . . . <span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                </ul>
                            </div>
                        </div>
                        <div class="col-lg-6 col-md-6 col-sm-6">
                            <div class="pricing-list">
                                <ul>
                                  <li>Rasta. . . . . . . . . . . <span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                    <li>Rasta. . . . . . . . . . .<span>25 000FCFA</span></li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
    </div>
    <!-- Best Pricing Area End -->
    <!--? Gallery Area Start -->
    <div class="gallery-area section-padding30">
        <div class="container">
            <!-- Section Tittle -->
            <div class="row justify-content-center">
                <div class="col-xl-6 col-lg-7 col-md-9 col-sm-10">
                    <div class="section-title text-center mb-100">
                        <span>our image gellary</span>
                        <h2>some images from our barber shop</h2>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-lg-4 col-md-6 col-sm-6">
                    <div class="box snake mb-30">
                        <div class="gallery-img gallery-img1"></div>
                    </div>
                </div>
                <div class="col-lg-8 col-md-6 col-sm-6">
                    <div class="box snake mb-30">
                        <div class="gallery-img gallery-img2"></div>
                    </div>
                </div>
                <div class="col-lg-8 col-md-6 col-sm-6">
                    <div class="box snake mb-30">
                        <div class="gallery-img gallery-img3"></div>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6 col-sm-6">
                    <div class="box snake mb-30">
                        <div class="gallery-img gallery-img4"></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- Gallery Area End -->

    <!-- Testimonial Details Start -->
    <div class="testimonial">

      <div class="testimonial-wrapper">
        <div class="quote-up">
          <span role="img" class="anticon">
            <svg width="4em" height="4em" viewBox="0 0 55 55" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M18.5395 26.6464H7.79159C7.97492 15.9443 10.0833 14.1798 16.6603 10.2839C17.4166 9.82559 17.6687 8.86309 17.2103 8.08392C16.7749 7.32767 15.7895 7.07559 15.0333 7.53392C7.28742 12.1173 4.58325 14.9131 4.58325 28.2277V40.5798C4.58325 44.4985 7.76867 47.661 11.6645 47.661H18.5395C22.5728 47.661 25.6208 44.6131 25.6208 40.5798V33.7048C25.6208 29.6943 22.5728 26.6464 18.5395 26.6464Z" fill="currentColor"></path>
              <path d="M43.3354 26.6464H32.5875C32.7708 15.9443 34.8791 14.1798 41.4562 10.2839C42.2125 9.82559 42.4645 8.86309 42.0062 8.08392C41.5479 7.32767 40.5854 7.07559 39.8062 7.53392C32.0604 12.1173 29.3562 14.9131 29.3562 28.2506V40.6027C29.3562 44.5214 32.5416 47.6839 36.4374 47.6839H43.3124C47.3458 47.6839 50.3937 44.636 50.3937 40.6027V33.7277C50.4166 29.6943 47.3687 26.6464 43.3354 26.6464Z" fill="currentColor"></path>
            </svg>
          </span>
        </div>
      </div>

      <div class="testimonial-content">
        <div class="ant-caroussel">
          <div class="slider">
            <div class="slider-list">
              

              <div id="carouselExample" class="carousel slide">
                <div class="carousel-inner">
                  <div class="carousel-item active">
                    <div><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span>
                    </div>
                    <h4 class="testimonial-title">That girl is too good</h4>
                    <p class="testimonial-text">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut facilis laborum, esse aut facere quidem! Rem doloribus quae.
                    </p>
                    <div class="testimonial-author">Ivana</div>
                    <!-- <img src="..." class="d-block w-100" alt="..."> -->
                  </div>
                  <div class="carousel-item">
                    <div><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span>
                    </div>
                    <h4 class="testimonial-title">I like it</h4>
                    <p class="testimonial-text">
                        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Numquam delectus nulla dolor vel accusantium, fugit hic ab impedit?
                    </p>
                    <div class="testimonial-author">Nathalia</div>
                  </div>
                  <div class="carousel-item">
                    <div><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span><span role="img" class="anticon star-icon"><svg width="3em" height="3em" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21.9995 9.66966C21.9363 9.48674 21.8215 9.32608 21.6688 9.20716C21.5162 9.08823 21.3323 9.01615 21.1395 8.99966L15.4495 8.16966L12.8995 2.99966C12.8176 2.83059 12.6898 2.688 12.5306 2.58823C12.3714 2.48846 12.1873 2.43555 11.9995 2.43555C11.8116 2.43555 11.6276 2.48846 11.4684 2.58823C11.3092 2.688 11.1814 2.83059 11.0995 2.99966L8.54949 8.15966L2.85949 8.99966C2.67441 9.02596 2.50041 9.10362 2.35724 9.22381C2.21407 9.34401 2.10745 9.50193 2.04949 9.67966C1.99643 9.85333 1.99167 10.0382 2.03572 10.2143C2.07976 10.3905 2.17095 10.5514 2.29949 10.6797L6.42949 14.6797L5.42949 20.3597C5.39379 20.5471 5.41248 20.7409 5.48336 20.9181C5.55424 21.0953 5.67434 21.2485 5.82949 21.3597C5.98071 21.4678 6.15906 21.5316 6.34454 21.5439C6.53001 21.5563 6.71526 21.5167 6.87949 21.4297L11.9995 18.7597L17.0995 21.4397C17.2398 21.5188 17.3983 21.5602 17.5595 21.5597C17.7713 21.5604 17.9779 21.4939 18.1495 21.3697C18.3046 21.2585 18.4247 21.1053 18.4956 20.9281C18.5665 20.7509 18.5852 20.5571 18.5495 20.3697L17.5495 14.6897L21.6795 10.6897C21.8239 10.5673 21.9306 10.4066 21.9872 10.226C22.0439 10.0455 22.0481 9.85253 21.9995 9.66966Z" fill="#FFD76E"></path></svg></span>
                    </div>
                    <h4 class="testimonial-title">Woooow amazing!!!</h4>
                    <p class="testimonial-text">
                        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Magnam vel eos praesentium cumque. At et cum sint unde!
                    </p>
                    <div class="testimonial-author">Lynn</div>
                  </div>
                </div>
                <div class="buttons">
                <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
                  <span aria-hidden="true" role="img" class="anticon"><svg width="1em" height="1em" viewBox="0 0 22 16" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M8.90382 0.353748C8.97693 0.426811 9.03493 0.513565 9.0745 0.609051C9.11407 0.704538 9.13443 0.806886 9.13443 0.910248C9.13443 1.01361 9.11407 1.11596 9.0745 1.21144C9.03493 1.30693 8.97693 1.39368 8.90382 1.46675L3.18581 7.187L20.7133 7.187C20.9222 7.187 21.1225 7.26997 21.2702 7.41765C21.4178 7.56534 21.5008 7.76564 21.5008 7.9745C21.5008 8.18336 21.4178 8.38366 21.2702 8.53134C21.1225 8.67903 20.9222 8.762 20.7133 8.762L3.18581 8.762L8.90382 14.4822C9.05141 14.6298 9.13433 14.83 9.13433 15.0387C9.13433 15.2475 9.05141 15.4477 8.90382 15.5952C8.75622 15.7428 8.55604 15.8258 8.34732 15.8258C8.13859 15.8258 7.93841 15.7428 7.79082 15.5952L0.728814 8.531L0.653814 8.4395L0.645564 8.42825L0.728814 8.531C0.664016 8.46573 0.61121 8.38957 0.572814 8.306L0.561564 8.2835C0.549692 8.25586 0.539425 8.22757 0.530814 8.19875C0.526314 8.17925 0.522564 8.1635 0.518814 8.147C0.512304 8.11979 0.507296 8.09225 0.503814 8.0645C0.503814 8.0465 0.503814 8.0285 0.499314 8.01125C0.494814 7.994 0.499314 7.98725 0.499314 7.9745L0.499314 7.93775C0.499314 7.92025 0.500814 7.90275 0.503814 7.88525L0.498564 7.9745C0.498427 7.9152 0.504968 7.85608 0.518064 7.79825C0.518064 7.784 0.524814 7.76975 0.529314 7.75625C0.537808 7.72666 0.548077 7.6976 0.560064 7.66925L0.578814 7.63775C0.61604 7.55655 0.666758 7.48225 0.728814 7.418L7.79457 0.353748C7.94197 0.207235 8.14136 0.125 8.34919 0.125C8.55702 0.125 8.75641 0.207235 8.90382 0.353748Z" fill="currentColor"></path></svg></span>
                  <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
                  <span aria-hidden="true" role="img" class="anticon"><svg width="1em" height="1em" viewBox="0 0 22 16" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M13.0962 15.6463C13.0231 15.5732 12.9651 15.4864 12.9255 15.3909C12.8859 15.2955 12.8656 15.1931 12.8656 15.0898C12.8656 14.9864 12.8859 14.884 12.9255 14.7886C12.9651 14.6931 13.0231 14.6063 13.0962 14.5333L18.8142 8.813L1.28668 8.813C1.07783 8.813 0.877522 8.73003 0.729836 8.58235C0.582152 8.43466 0.499182 8.23436 0.499182 8.0255C0.499182 7.81664 0.582152 7.61634 0.729836 7.46865C0.877522 7.32097 1.07783 7.238 1.28668 7.238L18.8142 7.238L13.0962 1.51775C12.9486 1.37016 12.8657 1.16998 12.8657 0.961253C12.8657 0.752526 12.9486 0.552345 13.0962 0.404753C13.2438 0.257159 13.444 0.174243 13.6527 0.174243C13.8614 0.174243 14.0616 0.25716 14.2092 0.404753L21.2712 7.469L21.3462 7.5605L21.3544 7.57175L21.2712 7.469C21.336 7.53427 21.3888 7.61043 21.4272 7.694L21.4384 7.7165C21.4503 7.74414 21.4606 7.77243 21.4692 7.80125C21.4737 7.82075 21.4774 7.8365 21.4812 7.853C21.4877 7.88021 21.4927 7.90775 21.4962 7.9355C21.4962 7.9535 21.4962 7.9715 21.5007 7.98875C21.5052 8.006 21.5007 8.01275 21.5007 8.0255L21.5007 8.06225C21.5007 8.07975 21.4992 8.09725 21.4962 8.11475L21.5014 8.0255C21.5016 8.0848 21.495 8.14392 21.4819 8.20175C21.4819 8.216 21.4752 8.23025 21.4707 8.24375C21.4622 8.27334 21.4519 8.3024 21.4399 8.33075L21.4212 8.36225C21.384 8.44345 21.3332 8.51775 21.2712 8.582L14.2054 15.6463C14.058 15.7928 13.8586 15.875 13.6508 15.875C13.443 15.875 13.2436 15.7928 13.0962 15.6463Z" fill="currentColor"></path></svg></span>
                  <span class="visually-hidden">Next</span>
                </button>
                </div>
              </div>
            
            </div>
            
          </div>
        </div>
        <img src="@/assets/QWYZ0059.png" class="testimonial-banner" alt="testimonial banner">
      </div>
    </div>
    <!-- Testimonial Details End -->
  </main>
</template>

<script setup>
  import { ref, onMounted } from 'vue';
  import AppointmentCard from '../components/AppointmentCard.vue';

  let show = ref(false)

  const showPopup = () => {
    show.value = !show.value
  }
</script>

<style>
.slider-area{
  width: 100%;
  height: 500px;
  background-image:url(../assets/YFXO7937.png);
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}
.slider-area .hero__caption{
  overflow:hidden;
}
@keyframes fade-in{
  0% {
    opacity:0.3;
    -webkit-transform:translate3d(0,100%,0);
    transform:translate3d(0,100%,0)
  }
  10% {
    opacity:0.5;
    -webkit-transform:translate3d(0,100%,0);
    transform:translate3d(0,100%,0)
  }
  20% {
    opacity:0.5;
    -webkit-transform:translate3d(0,100%,0);
    transform:translate3d(0,100%,0)
  }
  30% {
    opacity: 1;
    -webkit-transform:translateZ(0);
    transform:translateZ(0)
  }
  40% {
    opacity: 1;
    -webkit-transform:translateZ(0);
    transform:translateZ(0)
  }
  50% {
    opacity: 1;
    -webkit-transform:translateZ(0);
    transform:translateZ(0)
  }
  60% {
    opacity: 1;
    -webkit-transform:translateZ(0);
    transform:translateZ(0)
  }
  70% {
    opacity: 1;
    -webkit-transform:translateZ(0);
    transform:translateZ(0)
  }
  80% {
    opacity: 1;
    -webkit-transform:translateZ(0);
    transform:translateZ(0)
  }
  90% {
    opacity: 1;
    -webkit-transform:translateZ(0);
    transform:translateZ(0)
  }
  100% {
    opacity:1;
    -webkit-transform:translateZ(0);
    transform:translateZ(0)
  }
}

.slider-area .hero__caption span{
  overflow:hidden;
  font-size:40px;
  color:var(--secondary);
  font-weight:500;
  margin-top:26px;
  margin-bottom:26px;
  display:block;
  letter-spacing:0.08em;
  animation-name: fade-in;
  animation-delay: 2s;
  animation-duration: 7s;
  animation-timing-function: ease-in-out;
  animation-fill-mode: forwards;
  animation-iteration-count: infinite;
}
.slider-area .hero__caption h1{
  overflow:hidden;
  font-size:50px;
  font-weight:700;
  margin-bottom:14px;
  color:var(--secondary);
  line-height:1.4;
  text-transform:uppercase;
  animation-name: fade-in;
  animation-delay: 2s;
  animation-duration: 7s;
  animation-timing-function: ease-in;
  animation-fill-mode: forwards;
  animation-iteration-count: infinite;
}

.slider-area .stock-text{
  width:100%;
  margin-top: 10px;
}
.slider-area .stock-text h2{
  font-size:50px;
  font-weight:700;
  font-family:"Oswald",sans-serif;
  color:#eee;
  margin:0;
  line-height:1;
  text-transform:uppercase;
}
.slider-area .stock-text h2:nth-child(1){
  color:var(--secondary);
  -webkit-text-stroke:1px rgba(255,255,255,0.4);
  -webkit-text-fill-color:transparent;
}
  .slider-area .stock-text h2:nth-child(2){
    color:rgba(0, 191, 255, 0.6);
    -webkit-animation:animate 4s ease-in-out infinite;
    animation:animate 4s ease-in-out infinite;
    margin-top: -44px;
  }
  @keyframes animate{
    0%,100%{clip-path:polygon(0% 45%, 15% 44%, 32% 50%, 54% 60%, 70% 61%, 84% 69%, 100% 52%, 100% 100%, 0% 100%)}
    50%{clip-path:polygon(0% 60%, 16% 65%, 34% 66%, 51% 62%, 67% 50%, 84% 45%, 100% 46%, 100% 100%, 0% 100%)}
  }
  .slider-area .thumb-content-box{
    position:absolute;
    top:505px;
    right:0px;
    z-index:2;
    width:40%;
  }
  .slider-area .thumb-content-box .thumb-content{
    -webkit-box-align:end;
    -ms-flex-align:end;
    align-items:end;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-pack:justify;
    -ms-flex-pack:justify;
    justify-content:space-between;
    padding:30px 20px;
    width:100%;
    line-height:1;
    background:var(--primary);
  }
.slider-area .thumb-content-box .thumb-content h3{
  color:#000000;
  font-weight:600;
  font-size:18px;
  margin:0;
  text-transform:uppercase;
}
.slider-area .thumb-content-box .thumb-content i{
  font-size: 25px;
}
.about-area{
  margin-top: 10px;
}
.about-area .about-img img{
  display: flex;
  width:80%;
  margin: 0 auto;
  height: 450px;
  object-fit: cover;
  object-position: center;
}
.about-area .about-caption{
  padding-top:50px;
  padding-left:0;
}
.section-title span{
  font-size:16px;
  font-weight:600;
  margin-bottom:22px;
  color:var(--secondary);
  text-transform:uppercase;
  display:inline-block;
  letter-spacing:0.05em;
}
.section-tittle h2{
  font-size:50px;
  display:block;
  color:var(--secondary);
  font-weight:700;
  text-transform:uppercase;
}
.about-area .about-caption .pera-top{
  font-size:16px;
  font-weight:500;
  color:var(--secondary);
}
.about-area .about-caption .pera-bottom{
  font-size:16px;
  color:var(--secondary);
  font-weight:300;
}
.service-area{
  margin-top: 30px;
  padding-bottom:100px;
}
.service-area .services-caption{
  background:#f8f8f8;
  padding:84px 25px 56px;
  border-radius:7px;
  -webkit-transition:.5s;
  -moz-transition:.5s;
  -o-transition:.5s;
  transition:.5s;
  margin-bottom: 10px;
}
.service-area .services-caption .service-icon{
  display:inline-block;
  position:relative;
}
.service-area .services-caption .service-icon img{
  width: 205px;
  height: 150px;
  object-fit: cover;
  object-position: center;
  position:relative;
  display:block;
  margin-bottom:42px;
  -webkit-transition:.5s;
  -moz-transition:.5s;
  -o-transition:.5s;
  transition:.5s;
}
.service-area .services-caption .service-icon::before{
  background-image:url(../assets/dot.png);
  content:"";
  width:130px;
  height:135px;
  position:absolute;
  right:-45px;
  top:-25px;
  z-index:0;
  -webkit-transition:.5s;
  -moz-transition:.5s;
  -o-transition:.5s;
  transition:.5s;
}
.service-area .services-caption .service-cap h4{
  font-size:24px;
  font-weight:700;
  line-height:1.2;
  margin-bottom:27px;
  display:inline-block;
  color:var(--secondary);
}
.service-area .services-caption .service-cap h4:hover{
  color:var(--primary);
}
.services-caption:hover .service-icon::before{
  right:-20px;
  height:235px;
  width:150px;
}
.services-caption:hover .service-icon img{
  width: 255px;
  height: 250px;
}
.team-area{
  margin-top: 30px;
}
.team-area .carousel-indicators button{
  background-color: var(--secondary);
}
.team-area .carousel-item{
  position:relative
}

.team-area img{
  width:100%;
  height: 600px;
  object-fit: cover;
  object-position: center;
}
  .team-area .carousel-item .team-caption{
    background-image:url(../assets/team_bg.png);
    width:350px;
    height:155px;
    background-repeat:no-repeat;
    padding-top:57px;
    margin:0 auto;
    left:0;
    right:0;
    z-index:1;
    position:absolute;
    bottom:40px;
    -webkit-transition:.4s;
    -moz-transition:.4s;
    -o-transition:.4s;
    transition:.4s;
    background-size:contain
  }
  .team-area .carousel-item:hover{
    transform:scale(1.1);
    transition:all 0.6s ease-out 0s;
  }
  .team-area .carousel-item:hover .team-caption{
    background-image:url(../assets/team_bg2.png);
  }
.best-pricing{
  background:#fffcf9;
  margin-top: 30px;
}
.best-pricing .pricing-list ul li{
  font-family:"Oswald",sans-serif;
  text-transform:uppercase;
  font-size:14px;
  font-weight:500;
  color:#010101;
  margin-bottom:18px;
}
.best-pricing .pricing-list ul li span{
  color:#d19f68 !important;
  font-weight:400;
  font-size:16px;
}
.best-pricing .pricing-img{
  width: 100%;
}
.best-pricing .pricing-img .pricing-img1{
  width:100%;
}

.gallery-area .gallery-img{
  margin: 10px 0;
}

.gallery-area .gallery-img:hover{
  transform:scale(1.03);
  transition:all 0.6s ease-out 0s;
  opacity: 0.7;
}
.gallery-area .gallery-img1{
  background-image:url(../assets/WMUF5666.png);
  height: 400px;
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}

  .gallery-area .gallery-img2{
    background-image:url(../assets/TDTG9998.png);
    height: 500px;
    background-repeat:no-repeat;
    background-position:top center;
    background-position: center;
    background-size:cover;
  }

.gallery-area .gallery-img3{
  background-image:url(../assets/TMZX0632.png);
  height: 500px;
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}

.gallery-area .gallery-img4{
  background-image:url(../assets/PBKK5683.png);
  height: 400px;
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}
.gallery-area .gallery-img5{
  background-image:url(../assets/LCHV4107.png);
  height: 430px;
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}
.gallery-area .gallery-img6{
  background-image:url(../assets/HQWV9777.png);
  height: 530px;
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}
.gallery-area .gallery-img7{
  background-image:url(../assets/QWYZ0059.png);
  height: 450px;
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}
.gallery-area .gallery-img8{
  background-image:url(../assets/LPRA4797.png);
  height: 490px;
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}
.gallery-area .gallery-img9{
  background-image:url(../assets/KQDD8499.png);
  height: 510px;
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}
.gallery-area .gallery-img10{
  background-image:url(../assets/MHLZ0467.png);
  height: 390px;
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}
.gallery-area .gallery-img11{
  background-image:url(../assets/MGIJ1795.png);
  height: 430px;
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}
.gallery-area .gallery-img12{
  background-image:url(../assets/YFXO7937.png);
  height: 480px;
  background-repeat:no-repeat;
  background-position:top center;
  background-position: center;
  background-size:cover;
}

.testimonial{
    display: flex;
    width: 90%;
    margin-top: 50px;
}
.testimonial-wrapper{
    position: relative;
    border-radius: 15px;
    background-color: #fff;
    height: 80px;
    z-index: 2;
    margin: 0 auto;
}
.quote-up{
    position: absolute;
    top: 37px;
    left: -25px;
    display: flex;
    color: var(--primary);
    padding: 11px;
    box-shadow: rgba(12, 26, 75, 0.1) 0px 0px 1px, rgba(20, 37, 63, 0.06) 0px 10px 16px;
    border-radius: 12px;
    background-color: #fff;
    z-index: 3;
}
.anticon{
    display: inline-block;
    font-style: normal;
    line-height: 0;
    text-align: center;
    text-transform: none;
    vertical-align: -0.125em;
}
.testimonial-content{
    position: relative;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    background-color: #e9f4ff;
    padding: 40px 0px 35px 58px;
    width: 95%;
    border-radius: 35px;
}
.ant-caroussel{
    flex-basis: 55%;
    max-width: 55%;
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    color: #000;
    font-size: 14px;
    line-height: 1;
    list-style: none;
}
.testimonial-banner {
    flex-basis: 45%;
    max-width: 45%;
    height: 100%;
    position: absolute;
    bottom: 0px;
    right: 0px;
    border-radius: 35px;
    border-top-left-radius: 0;
    border-bottom-left-radius: 0;
    object-fit: cover;
    object-position: center;
    width: 80%;
}

.testimonial-title{
    font-weight: 700;
    font-size: 18px;
    line-height: 22px;
    margin: 10px 0px 12px;
    color: #2d1f21;
}
.testimonial-text{
    font-weight: 400;
    font-size: 15px;
    line-height: 25px;
    margin-bottom: 16px;
    color: #2d1f21;
    width: 85%;
}
.testimonial-author{
    position: relative;
    font-weight: 700;
    font-size: 16px;
    line-height: 14px;
    color: #857e7f;
    padding-left: 16px;  
}
.testimonial-author::before {
    content: "";
    position: absolute;
    top: 0px;
    bottom: 0px;
    left: 0px;
    width: 6px;
    background-color: var(--secondary);
    border-radius: 6px;
}
.testimonial-author p{
    font-weight: 700;
    font-size: 16px;
    line-height: 14px;
    color: #857e7f;
    padding-left: 16px;
}
.buttons{
    display: flex;
    margin-top: 50px;

}
.buttons button{
    border: none;
    border-radius: 50%;
    display: flex;
    -webkit-box-align: center;
    align-items: center;
    -webkit-box-pack: center;
    justify-content: center;
    bottom: -20px;
    z-index: 4;
    background: rgb(255, 255, 255) !important;
    color: #aba7a7 !important;
    font-size: unset !important;
    width: 48px !important;
    height: 48px !important;
    margin-top: 60px !important;
    top: unset !important;
    margin-right: 0px;
}

.buttons .carousel-control-next{
  left: 70px !important;
}


@media (max-width: 850px){
  .slider-area{
    height: 400px;
  }
  .slider-area .hero__caption span{
  font-size:30px;
  margin-top:26px;
  margin-bottom:20px;
}
.slider-area .hero__caption h1{
  overflow:hidden;
  font-size:40px;
  margin-bottom:10px;
}

  .slider-area .stock-text h2{
    font-size:30px
  }
  .slider-area .stock-text h2:nth-child(2){
    margin-top: -30px;
  }
  .slider-area .thumb-content-box{
    width:45%;
    top: 399px;
  }
  .slider-area .thumb-content-box .thumb-content{
    padding:20px 20px;
  }
  .slider-area .thumb-content-box .thumb-content h3{
    font-size:15px;
  }
  .service-area{
    padding-bottom:70px;
  }
  .best-pricing .pricing-img{
    padding-top:60px;
  }
  .best-pricing .pricing-img .pricing-img1{
    position:unset;
    width:80%;
    height:450px;
  }
  .gallery-area .gallery-img3{
    margin-top: -40px;
  }
  
}

@media (max-width: 691px){
  .slider-area{
    height: 300px;
  }
  .slider-area .hero__caption span{
  font-size:20px;
  margin-top:26px;
  margin-bottom:20px;
}
.slider-area .hero__caption h1{
  overflow:hidden;
  font-size:30px;
  margin-bottom:10px;
}

.slider-area .stock-text h2{
  font-size:20px;
}
.slider-area .stock-text h2:nth-child(2){
    margin-top: -20px;
  }
  .slider-area .thumb-content-box{
    width: 60%;
    top: 325px;
  }
  .slider-area .thumb-content-box .thumb-content{
    padding:10px 10px;
  }
  .slider-area .thumb-content-box .thumb-content h3{
    font-size:10px;
  }
  .slider-area .thumb-content-box .thumb-content i{
    font-size: 15px;
  }
  .about-area .about-caption{
  padding-top:40px;
}

.best-pricing .pricing-img .pricing-img1{
  position:unset;
  width:90%;
  height:320px;
}
.gallery-area .gallery-img1{
  height: 200px;
}

  .gallery-area .gallery-img2{
    height: 200px;
  }

.gallery-area .gallery-img3{
  height: 200px;
}

.gallery-area .gallery-img4{
  height: 200px;
}
.gallery-area .gallery-img3{
    margin-top: 10px;
  }
.testimonial{
    margin-top: 50px;
}
.testimonial-wrapper{
    height: 30px;
}
.quote-up{
    top: 27px;
    left: -5px;
    padding: 8px;
}
.quote-up span svg{
  width: 2em !important;
  height: 2em !important;
}
.carousel-item span svg{
  width: 1.5em !important;
  height: 1.5em !important;
}

.testimonial-title{
    font-size: 14px;
}
.testimonial-text{
    font-size: 12px;
}
.testimonial-author{
    font-size: 12px;
}

.testimonial-author p{
    font-size: 14px;
}

}
</style>
