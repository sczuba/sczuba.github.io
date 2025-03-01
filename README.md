<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <meta http-equiv="X-UA-Compatible" content="ie=edge" />
        <meta name="keywords" content="Document" />
        <meta name="description" content="Your Description..." />
        <title>Document</title>
        <link
            rel="stylesheet"
            href="/resources/swiper-js/swiper-bundle.min.css" />
        <link
            rel="stylesheet"
            href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/css/all.min.css" />
        <link rel="stylesheet" href="/resources/css/loader.css" />
        <link rel="stylesheet" href="/resources/css/hamburger.css" />
        <link rel="stylesheet" href="/resources/css/home.css" />
        <link rel="stylesheet" href="/resources/css/about.css" />
        <link rel="stylesheet" href="/resources/css/services.css" />
        <link rel="stylesheet" href="/resources/css/portfolio.css" />
        <link rel="stylesheet" href="/resources/css/comments.css" />
        <link rel="stylesheet" href="/resources/css/contact.css" />
        <link href="/resources/mapbox-gl/mapbox-gl.css" rel="stylesheet" />
        <link rel="stylesheet" href="/resources/css/style.css" />
        <link
            rel="shortcut icon"
            href="/resources/img/favicon.ico"
            type="image/x-icon" />
    </head>
    <body onload="loaded()">
        <div class="loader">
            <div class="c c1"></div>
            <div class="c c2"></div>
            <div class="c c3"></div>
            <div class="c c4"></div>
            <div class="c c5"></div>
            <div class="c c6"></div>
        </div>
        <script>
            let loader = document.querySelector(".loader");
            function loaded() {
                loader.classList.add("remove");
                setTimeout(() => {
                    loader.style.display = "none";
                }, 1000);
            }
        </script>
        <!-- HAMBURGER MENU BUTTON (responsively visible) -->
        <div class="hamburger">
            <div class="bar1"></div>
            <div class="bar2"></div>
            <div class="bar3"></div>
        </div>

        <!-- THE REAL NAVIGATION -->
        <nav class="navigation">
            <h1>
                Shuvro
                <div></div>
                <div></div>
            </h1>
            <ul>
                <li><a href="#" onclick="home()">home</a></li>
                <li>
                    <a
                        href="#"
                        onclick="about(); animate3.play(); animate4.play();"
                        >about</a
                    >
                </li>
                <li>
                    <a href="#" onclick="services(); animate6.play();"
                        >services</a
                    >
                </li>
                <li><a href="#" onclick="portfolio()">portfolio</a></li>
                <li><a href="#" onclick="comments()">comments</a></li>
                <li>
                    <a href="#" onclick="contact(); animate5.play()">contact</a>
                </li>
            </ul>
            <p>
                &copy; 2024
                <a
                    href="https://github.com/shu-vro"
                    target="_blank"
                    rel="noopener noreferrer"
                    >Shuvro</a
                >.
            </p>
        </nav>

        <div class="container">
            <div class="layer layer1 active">
                <div class="home main">
                    <div class="canvas_container">
                        <canvas></canvas>
                    </div>
                    <div class="content-for-home">
                        <div class="img-container"></div>
                        <h1 align="center">Shirshen Das Gupta Shuvro</h1>
                        <div class="social-icons">
                            <div class="s-icon">
                                <a href="#">
                                    <i class="fab fa-facebook"></i>
                                </a>
                                <div class="s-name">Facebook</div>
                            </div>
                            <div class="s-icon">
                                <a href="#">
                                    <i class="fab fa-twitter"></i>
                                </a>
                                <div class="s-name">Tweeter</div>
                            </div>
                            <div class="s-icon">
                                <a href="#">
                                    <i class="fab fa-github"></i>
                                </a>
                                <div class="s-name">GitHub</div>
                            </div>
                            <div class="s-icon">
                                <a href="#">
                                    <i class="fab fa-codepen"></i>
                                </a>
                                <div class="s-name">CodePen</div>
                            </div>
                            <div class="s-icon">
                                <a href="#">
                                    <i class="fab fa-instagram"></i>
                                </a>
                                <div class="s-name">Instagram</div>
                            </div>
                            <div class="s-icon">
                                <a href="#">
                                    <i class="fas fa-envelope"></i>
                                </a>
                                <div class="s-name">Email</div>
                            </div>
                        </div>

                        <div class="side-nav">
                            <button
                                onclick="about(); animate3.play(); animate4.play();">
                                <span class="w">W</span>
                                <span class="tooltip"> why you? </span>
                            </button>
                            <button onclick="services(); animate6.play();">
                                <span class="w">W</span>
                                <span class="tooltip"> what do you do? </span>
                            </button>
                            <button onclick="portfolio()">
                                <span class="w">W</span>
                                <span class="tooltip">
                                    what have you done?
                                </span>
                            </button>
                            <button onclick="comments()">
                                <span class="w">W</span>
                                <span class="tooltip"> what others say? </span>
                            </button>
                            <button onclick="contact(); animate5.play()">
                                <span class="w">W</span>
                                <span class="tooltip"> where are you? </span>
                            </button>
                        </div>

                        <div class="titles-for-side-nav">
                            <span></span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="layer layer2">
                <div class="about main">
                    <!-- SEGMENT FOR STYLING. -->
                    <div class="styling">
                        <div class="absolute box"></div>
                        <div class="absolute circle"></div>
                        <div class="absolute triangle"></div>
                        <div class="absolute dots">
                            <div class="dot dot1"></div>
                            <div class="dot dot2"></div>
                            <div class="dot dot3"></div>
                            <div class="dot dot4"></div>
                            <div class="dot dot5"></div>
                            <div class="dot dot6"></div>
                            <div class="dot dot7"></div>
                            <div class="dot dot8"></div>
                            <div class="dot dot9"></div>
                            <div class="dot dot10"></div>
                            <div class="dot dot11"></div>
                            <div class="dot dot12"></div>
                            <div class="dot dot13"></div>
                            <div class="dot dot14"></div>
                            <div class="dot dot15"></div>
                            <div class="dot dot16"></div>
                            <div class="dot dot17"></div>
                            <div class="dot dot18"></div>
                            <div class="dot dot19"></div>
                            <div class="dot dot20"></div>
                            <div class="dot dot21"></div>
                            <div class="dot dot22"></div>
                            <div class="dot dot23"></div>
                            <div class="dot dot24"></div>
                        </div>

                        <svg
                            class="wave absolute"
                            xmlns="http://www.w3.org/2000/svg"
                            viewBox="0 0 1450 320">
                            <path
                                fill-opacity="1"
                                d="M0,320L48,277.3C96,235,192,149,288,122.7C384,96,480,128,576,165.3C672,203,768,245,864,234.7C960,224,1056,160,1152,112C1248,64,1344,32,1392,16L1440,0L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path>
                        </svg>

                        <svg
                            class="wave absolute opposite"
                            xmlns="http://www.w3.org/2000/svg"
                            viewBox="0 0 1450 320">
                            <path
                                fill-opacity="1"
                                d="M0,224L48,213.3C96,203,192,181,288,192C384,203,480,245,576,218.7C672,192,768,96,864,64C960,32,1056,64,1152,101.3C1248,139,1344,181,1392,202.7L1440,224L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path>
                        </svg>
                    </div>

                    <!-- REAL CONTENT -->
                    <div class="wrapper">
                        <div class="face face1">
                            <div class="content">
                                <p>Hello,</p>
                                <h1>I'm Shuvro</h1>
                                <p class="text">
                                    I am a Web Developer, and I'm very
                                    passionate and dedicated to my work With 10
                                    years experience as a professional Web
                                    Developer, I have acquired the skills and
                                    knowledge necessary to make your project a
                                    success I enjoy every step of the design
                                    process, from discussion and collaboration.
                                </p>
                                <a
                                    class="button download"
                                    href="/resources/img/bg1.png"
                                    download="shuvro_cv"
                                    >Download CV</a
                                >
                                <a
                                    class="button hire"
                                    href="#"
                                    class="hire"
                                    onclick="contact(); animate5.play()"
                                    >Hire Me.</a
                                >
                            </div>
                        </div>
                        <div class="face face2"></div>
                    </div>

                    <!-- THE NAVIGATION OF ABOUT -->
                    <nav class="about_nav">
                        <ul>
                            <li>
                                <a class="active" href="#" data-text="one"
                                    >Skills</a
                                >
                            </li>
                            <li>
                                <a href="#" data-text="two">Experience</a>
                            </li>
                            <li>
                                <a href="#" data-text="three">Education</a>
                            </li>
                        </ul>
                    </nav>

                    <div class="about_container">
                        <!-- SKILL BOX -->
                        <div class="skills">
                            <div class="skill">
                                <div class="name">HTML5</div>
                                <div class="value" style="left: 90%">90%</div>
                                <div class="percent">
                                    <div
                                        class="progress"
                                        style="width: 90%"></div>
                                </div>
                            </div>
                            <div class="skill">
                                <div class="name">CSS3</div>
                                <div class="value" style="left: 75%">75%</div>
                                <div class="percent">
                                    <div
                                        class="progress"
                                        style="width: 75%"></div>
                                </div>
                            </div>
                            <div class="skill">
                                <div class="name">JavaScript</div>
                                <div class="value" style="left: 65%">65%</div>
                                <div class="percent">
                                    <div
                                        class="progress"
                                        style="width: 65%"></div>
                                </div>
                            </div>
                            <div class="skill">
                                <div class="name">PHP</div>
                                <div class="value" style="left: 50%">50%</div>
                                <div class="percent">
                                    <div
                                        class="progress"
                                        style="width: 50%"></div>
                                </div>
                            </div>
                            <div class="skill">
                                <div class="name">Jquery</div>
                                <div class="value" style="left: 45%">45%</div>
                                <div class="percent">
                                    <div
                                        class="progress"
                                        style="width: 45%"></div>
                                </div>
                            </div>
                            <div class="skill">
                                <div class="name">C++</div>
                                <div class="value" style="left: 55%">55%</div>
                                <div class="percent">
                                    <div
                                        class="progress"
                                        style="width: 55%"></div>
                                </div>
                            </div>
                        </div>

                        <!-- EXPERIENCE -->
                        <div class="experience">
                            <div class="middle_line"></div>
                            <div class="cover">
                                <i class="job_box fas fa-briefcase"></i>
                                <i class="date">Sep 2020 - Present</i>
                                <h2>Full Stack Developer</h2>
                                <i class="name_company">Company Name</i>
                                <article class="text_hidden">
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Ut sint magnam ipsam
                                    eveniet omnis nemo commodi dolorum neque
                                    fugiat, soluta tempora vitae error magni.
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Quaerat est amet
                                    voluptatibus, nam perferendis provident
                                    veritatis cum, dolorum eaque voluptates
                                    asperiores, nostrum voluptatum. Autem
                                    incidunt praesentium tempora, minus suscipit
                                    fugiat?
                                </article>
                            </div>
                            <div class="whitespace"></div>
                            <div class="whitespace"></div>
                            <div class="cover">
                                <i class="job_box fas fa-briefcase"></i>
                                <i class="date">Apr 2020 - Jan 2019</i>
                                <h2>Full Stack Developer</h2>
                                <i class="name_company">Company Name</i>
                                <article class="text_hidden">
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Ut sint magnam ipsam
                                    eveniet omnis nemo commodi dolorum neque
                                    fugiat, soluta tempora vitae error magni.
                                </article>
                            </div>
                            <div class="cover">
                                <i class="job_box fas fa-briefcase"></i>
                                <i class="date">Feb 2018 - Apr 2020</i>
                                <h2>Full Stack Developer</h2>
                                <i class="name_company">Company Name</i>
                                <article class="text_hidden">
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Ut sint magnam ipsam
                                    eveniet omnis nemo commodi dolorum neque
                                    fugiat, soluta tempora vitae error magni.
                                </article>
                            </div>
                            <div class="whitespace"></div>
                            <div class="whitespace"></div>
                            <div class="cover">
                                <i class="job_box fas fa-briefcase"></i>
                                <i class="date">Aug 2014 - Feb 2018</i>
                                <h2>Full Stack Developer</h2>
                                <i class="name_company">Company Name</i>
                                <article class="text_hidden">
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Ut sint magnam ipsam
                                    eveniet omnis nemo commodi dolorum neque
                                    fugiat, soluta tempora vitae error magni.
                                </article>
                            </div>
                        </div>
                        <div class="education">
                            <div class="middle_line"></div>
                            <div class="cover">
                                <i class="job_box fas fa-book-reader"></i>
                                <i class="date">2019 - 2019</i>
                                <h2>Completed Graphics Designing</h2>
                                <i class="name_company">Google LLC.</i>
                                <article class="text_hidden">
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Ut sint magnam ipsam
                                    eveniet omnis nemo commodi dolorum neque
                                    fugiat, soluta tempora vitae error magni.
                                </article>
                            </div>
                            <div class="whitespace"></div>
                            <div class="whitespace"></div>
                            <div class="cover">
                                <i class="job_box fas fa-book-reader"></i>
                                <i class="date">2018 - 2019</i>
                                <h2>Completed Web Designing Course</h2>
                                <i class="name_company">Wixframe Inc.</i>
                                <article class="text_hidden">
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Ut sint magnam ipsam
                                    eveniet omnis nemo commodi dolorum neque
                                    fugiat, soluta tempora vitae error magni.
                                </article>
                            </div>
                            <div class="cover">
                                <i class="job_box fas fa-book-open"></i>
                                <i class="date">2016 - 2018</i>
                                <h2>Masters In Science</h2>
                                <i class="name_company">BUET, Bangladesh</i>
                                <article class="text_hidden">
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Ut sint magnam ipsam
                                    eveniet omnis nemo commodi dolorum neque
                                    fugiat, soluta tempora vitae error magni.
                                </article>
                            </div>
                            <div class="whitespace"></div>
                            <div class="whitespace"></div>
                            <div class="cover">
                                <i class="job_box fas fa-book-open"></i>
                                <i class="date">2012 - 2016</i>
                                <h2>Bachelor In Science</h2>
                                <i class="name_company">BUET, Bangladesh.</i>
                                <article class="text_hidden">
                                    Lorem ipsum dolor sit amet consectetur
                                    adipisicing elit. Ut sint magnam ipsam
                                    eveniet omnis nemo commodi dolorum neque
                                    fugiat, soluta tempora vitae error magni.
                                </article>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="layer layer3">
                <div class="services main">
                    <!-- <section class="background">
                        <div class="bg_wrapper"></div>
                    </section> -->
                    <div class="hero">
                        <span class="typography">
                            <span class="t_dummy">We know how to</span> <br />
                            <span class="t-box">
                                <span class="box-side box-front"
                                    >take risk</span
                                >
                                <span class="box-side box-top"
                                    >take a side</span
                                >
                                <span class="box-side box-back"
                                    >be different</span
                                >
                                <span class="box-side box-bottom"
                                    >be innovative</span
                                >
                            </span>
                        </span>
                        <p class="hero-text">
                            Shuvro is an excellent web designer and faultless
                            technician. He’s a pleasure to work with, great
                            value for money and will always go the extra mile
                            when necessary.
                        </p>
                    </div>
                    <div class="capabilities left move-little-down">
                        <img src="/resources/img/elements/web_bg.png" alt="" />
                        <p class="c_content">
                            <span class="c_title">Web</span>
                            His creative journey started with Web Design. To
                            code his own designs, he learned how to code and has
                            since then worked hard to stay relevant in both
                            fields. For smooth collaboration with clients he is
                            now-a-days using programing languages for designing
                            and prototyping.
                            <br />
                            <a href="#">Learn More</a>
                            <i class="far fa-arrow-alt-circle-right"></i>
                        </p>
                    </div>
                    <div class="capabilities right">
                        <p class="c_content">
                            <span class="c_title">Graphics</span>
                            With a designers eye for details, Shuvro is
                            passionate about implementing designed into highly
                            interactive experience by paying close attention to
                            details, animations and performances.
                            <br />
                            <a href="#">Learn More</a>
                            <i class="far fa-arrow-alt-circle-right"></i>
                        </p>
                        <img
                            src="/resources/img/elements/graphics_bg.png"
                            alt="" />
                    </div>
                    <div class="capabilities left">
                        <img
                            src="/resources/img/elements/seo_bg.png"
                            alt=""
                            style="
                                background: #2929292f;
                                backdrop-filter: blur(4px);
                                border-radius: 40px;
                            " />
                        <p class="c_content">
                            <span class="c_title">SEO</span>
                            With 1+ years of experience in the Digital industry,
                            he proved that the combination of strategic thinking
                            and expertise will create a fascinating digital
                            experience.
                            <br />
                            <a href="#">Learn More</a>
                            <i class="far fa-arrow-alt-circle-right"></i>
                        </p>
                    </div>
                    <div class="foot">
                        <h2>Works:</h2>
                        <div class="foot-link">
                            <a href="#" onclick="portfolio()">Profile World</a>
                            <i class="far fa-arrow-alt-circle-right"></i>
                            <img
                                src="/resources/img/portfolios/app/2.jpg"
                                alt="portfolio" />
                        </div>
                        <div class="foot-link">
                            <a href="#" onclick="portfolio()">Art Director</a>
                            <i class="far fa-arrow-alt-circle-right"></i>
                            <img
                                src="/resources/img/portfolios/card/2.jpg"
                                alt="portfolio" />
                        </div>
                        <div class="foot-link">
                            <a href="#" onclick="portfolio()">Lora Website</a>
                            <i class="far fa-arrow-alt-circle-right"></i>
                            <img
                                src="/resources/img/portfolios/web/1.jpg"
                                alt="portfolio" />
                        </div>
                    </div>
                </div>
            </div>
            <div class="layer layer4">
                <div class="portfolio main">
                    <div class="tip main">
                        <div class="allContent">
                            <div class="description" style="display: none">
                                <div class="pro_intro">
                                    <div class="nameplate">
                                        <h1>Wedding Couple</h1>
                                        <span
                                            >Category:
                                            <span style="color: #999"
                                                >Web Design</span
                                            ></span
                                        >
                                    </div>
                                    <div class="other_text">
                                        <h2>Project Brief:</h2>
                                        <p
                                            class="pro_brief"
                                            style="
                                                color: #999;
                                                padding-left: 15px;
                                            ">
                                            Lorem ipsum, dolor sit amet
                                            consectetur adipisicing elit. At
                                            corrupti modi perferendis iure
                                            corporis dolores minus asperiores
                                            nemo debitis veritatis id placeat,
                                            similique eum recusandae ipsa quia
                                            cum earum nam?
                                        </p>
                                    </div>
                                </div>
                                <div class="pro_info">
                                    <h2>Project Info</h2>
                                    <p class="Date">
                                        <b>Date: </b>
                                        <span style="color: #999">2020</span>
                                    </p>
                                    <p class="client">
                                        <b>Client: </b>
                                        <span style="color: #999">xyz</span>
                                    </p>
                                    <p>
                                        <b>Tools: </b>
                                        <span style="color: #999"
                                            >HTML, CSS, JavaScript</span
                                        >
                                    </p>
                                    <p class="link">
                                        <b>Web: </b>
                                        <span style="color: #999"
                                            ><a href="#"
                                                >www.domain.com</a
                                            ></span
                                        >
                                    </p>
                                </div>
                            </div>

                            <button class="closeButton">
                                <span>Project Details</span>
                                <div class="icon"></div>
                            </button>
                            <button class="exitButton">&times;</button>

                            <div class="port_content">
                                <div class="swiper-container-2">
                                    <div class="swiper-wrapper">
                                        <div class="swiper-slide">
                                            <img src="#" alt="web design" />
                                        </div>
                                        <div class="swiper-slide">
                                            <img src="#" alt="web design" />
                                        </div>
                                        <div class="swiper-slide">
                                            <img src="#" alt="web design" />
                                        </div>
                                        <div class="swiper-slide">
                                            <img src="#" alt="web design" />
                                        </div>
                                        <div class="swiper-slide">
                                            <img src="#" alt="web design" />
                                        </div>
                                        <div class="swiper-slide">
                                            <img src="#" alt="web design" />
                                        </div>
                                        <div class="swiper-slide">
                                            <img src="#" alt="web design" />
                                        </div>
                                        <div class="swiper-slide">
                                            <img src="#" alt="web design" />
                                        </div>
                                        <div class="swiper-slide">
                                            <img src="#" alt="web design" />
                                        </div>
                                    </div>
                                    <!-- Add Pagination -->
                                    <div class="swiper-scrollbar"></div>
                                    <!-- Add Arrows -->
                                    <div class="swiper-button-next"></div>
                                    <div class="swiper-button-prev"></div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <nav class="about_nav padding_top">
                        <ul>
                            <li>
                                <a
                                    class="filter active"
                                    href="#"
                                    data-filter="all"
                                    >All</a
                                >
                            </li>
                            <li>
                                <a class="filter" href="#" data-filter=".web"
                                    >Web Design</a
                                >
                            </li>
                            <li>
                                <a class="filter" href="#" data-filter=".logo"
                                    >Logo</a
                                >
                            </li>
                            <li>
                                <a class="filter" href="#" data-filter=".card"
                                    >Cards</a
                                >
                            </li>
                            <li>
                                <a class="filter" href="#" data-filter=".app"
                                    >Apps</a
                                >
                            </li>
                            <li>
                                <a class="filter" href="#" data-filter=".icon"
                                    >Icons</a
                                >
                            </li>
                        </ul>
                    </nav>
                    <div class="mymixcont">
                        <div class="mix web">
                            <img
                                src="/resources/img/portfolios/web/1.jpg"
                                alt="" />
                            <span class="title">Lora Website</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix icon">
                            <img
                                src="/resources/img/portfolios/icon/5.jpg"
                                alt="" />
                            <span class="title">Water World</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix card">
                            <img
                                src="/resources/img/portfolios/card/1.jpg"
                                alt="" />
                            <span class="title">Brand Photography</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix web">
                            <img
                                src="/resources/img/portfolios/web/2.jpg"
                                alt="" />
                            <span class="title">Student Guide</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix app">
                            <img
                                src="/resources/img/portfolios/app/1.jpg"
                                alt="" />
                            <span class="title">World View</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix card">
                            <img
                                src="/resources/img/portfolios/card/2.jpg"
                                alt="" />
                            <span class="title">Art Director</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix web">
                            <img
                                src="/resources/img/portfolios/web/3.jpg"
                                alt="" />
                            <span class="title">Web App Pro</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix card">
                            <img
                                src="/resources/img/portfolios/card/3.jpg"
                                alt="" />
                            <span class="title">Reauty</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix web">
                            <img
                                src="/resources/img/portfolios/web/4.jpg"
                                alt="" />
                            <span class="title">Sonor Design</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix card">
                            <img
                                src="/resources/img/portfolios/card/4.jpg"
                                alt="" />
                            <span class="title">Richard Tan</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix logo">
                            <img
                                src="/resources/img/portfolios/logo/1.jpg"
                                alt="" />
                            <span class="title">Kitty Pic</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix icon">
                            <img
                                src="/resources/img/portfolios/icon/4.jpg"
                                alt="" />
                            <span class="title">Domine</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix app">
                            <img
                                src="/resources/img/portfolios/app/2.jpg"
                                alt="" />
                            <span class="title">Profile World</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix logo">
                            <img
                                src="/resources/img/portfolios/logo/2.jpg"
                                alt="" />
                            <span class="title">Specialisterne</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix logo">
                            <img
                                src="/resources/img/portfolios/logo/3.jpg"
                                alt="" />
                            <span class="title">Native Design</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix card">
                            <img
                                src="/resources/img/portfolios/card/5.jpg"
                                alt="" />
                            <span class="title">Sriram Mohan</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix logo">
                            <img
                                src="/resources/img/portfolios/logo/4.jpg"
                                alt="" />
                            <span class="title">Book Worm</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix icon">
                            <img
                                src="/resources/img/portfolios/icon/2.jpg"
                                alt="" />
                            <span class="title">Football FC</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix logo">
                            <img
                                src="/resources/img/portfolios/logo/5.jpg"
                                alt="" />
                            <span class="title">Free Notes</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix icon">
                            <img
                                src="/resources/img/portfolios/icon/1.jpg"
                                alt="" />
                            <span class="title">Insta Genre</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix logo">
                            <img
                                src="/resources/img/portfolios/logo/6.jpg"
                                alt="" />
                            <span class="title">Movie Sock</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix logo">
                            <img
                                src="/resources/img/portfolios/logo/7.jpg"
                                alt="" />
                            <span class="title">Village Community Church</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix app">
                            <img
                                src="/resources/img/portfolios/app/3.jpg"
                                alt="" />
                            <span class="title">Weathery</span>
                            <span class="port_link">View Project</span>
                        </div>
                        <div class="mix icon">
                            <img
                                src="/resources/img/portfolios/icon/3.jpg"
                                alt="" />
                            <span class="title">Fav Shop</span>
                            <span class="port_link">View Project</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="layer layer5">
                <div class="testimonial">
                    <h1>
                        <span>See What My Clients Say about Me.</span>
                    </h1>
                    <div class="swiper-container">
                        <div class="swiper-wrapper">
                            <div class="swiper-slide">
                                <img src="/resources/img/favicon.ico" alt="" />
                                <h4>Erik Lasher</h4>
                                <div class="rating">
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                </div>
                                <p>
                                    <span>&ldquo;</span>
                                    Shuvro is an excellent web designer and
                                    faultless technician. He’s a pleasure to
                                    work with, great value for money and will
                                    always go the extra mile when necessary.
                                </p>
                            </div>
                            <div class="swiper-slide">
                                <img src="/resources/img/favicon.ico" alt="" />
                                <h4>Erik Lasher</h4>
                                <div class="rating">
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                </div>
                                <p>
                                    <span>&ldquo;</span>
                                    Shuvro is an excellent web designer and
                                    faultless technician. He’s a pleasure to
                                    work with, great value for money and will
                                    always go the extra mile when necessary.
                                </p>
                            </div>
                            <div class="swiper-slide">
                                <img src="/resources/img/favicon.ico" alt="" />
                                <h4>Erik Lasher</h4>
                                <div class="rating">
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                </div>
                                <p>
                                    <span>&ldquo;</span>
                                    Shuvro is an excellent web designer and
                                    faultless technician. He’s a pleasure to
                                    work with, great value for money and will
                                    always go the extra mile when necessary.
                                </p>
                            </div>
                            <div class="swiper-slide">
                                <img src="/resources/img/favicon.ico" alt="" />
                                <h4>Erik Lasher</h4>
                                <div class="rating">
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                </div>
                                <p>
                                    <span>&ldquo;</span>
                                    Shuvro is an excellent web designer and
                                    faultless technician. He’s a pleasure to
                                    work with, great value for money and will
                                    always go the extra mile when necessary.
                                </p>
                            </div>
                            <div class="swiper-slide">
                                <img src="/resources/img/favicon.ico" alt="" />
                                <h4>Erik Lasher</h4>
                                <div class="rating">
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                </div>
                                <p>
                                    <span>&ldquo;</span>
                                    Shuvro is an excellent web designer and
                                    faultless technician. He’s a pleasure to
                                    work with, great value for money and will
                                    always go the extra mile when necessary.
                                </p>
                            </div>
                            <div class="swiper-slide">
                                <img src="/resources/img/favicon.ico" alt="" />
                                <h4>Erik Lasher</h4>
                                <div class="rating">
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                    <label>&starf;</label>
                                </div>
                                <p>
                                    <span>&ldquo;</span>
                                    Shuvro is an excellent web designer and
                                    faultless technician. He’s a pleasure to
                                    work with, great value for money and will
                                    always go the extra mile when necessary.
                                </p>
                            </div>
                        </div>
                        <!-- Add Pagination -->
                        <div class="swiper-pagination"></div>
                        <div class="swiper-button-next"></div>
                        <div class="swiper-button-prev"></div>
                    </div>
                </div>
            </div>
            <div class="layer layer6">
                <div class="contact_us">
                    <div id="map"></div>
                    <address class="info_container">
                        <div class="info info1">
                            <i class="fas fa-phone-alt"></i>
                            <span class="iname">Phone</span>
                            <a href="tel:+8800000000000">+8800000000000</a>
                            <a href="tel:+8811111111111">+8811111111111</a>
                        </div>
                        <div class="info info2">
                            <i class="fas fa-home"></i>
                            <span class="iname">Address</span>
                            <a
                                href="https://www.google.com/maps/place/Sherpur+Town+Hall/@25.0136644,90.0140045,355m/data=!3m1!1e3!4m5!3m4!1s0x3757d6136d793499:0x8c22620664dc6a37!8m2!3d25.0156371!4d90.0168872">
                                <h3>Govt. Girls' School Road</h3>
                                <span>Kharampur, Sherpur</span><br />
                                <span>Bangladesh</span>
                            </a>
                        </div>
                        <div class="info info3">
                            <i class="fas fa-envelope"></i>
                            <span class="iname">Email</span>
                            <a href="mailto:email1.gmail.com"
                                >shuvro1@gmail.com</a
                            >
                            <a href="mailto:email2.gmail.com"
                                >shuvro2@gmail.com</a
                            >
                        </div>
                    </address>

                    <form action="#" method="post">
                        <h1>Get In Touch</h1>
                        <div class="inp_field">
                            <i class="fas fa-user"></i>
                            <input
                                type="text"
                                name="name"
                                class="fname"
                                id="fname"
                                placeholder="Full Name"
                                required />
                        </div>
                        <div class="inp_field">
                            <i class="fas fa-envelope"></i>
                            <input
                                type="email"
                                name="email"
                                class="email"
                                id="email"
                                placeholder="Email"
                                required />
                        </div>
                        <div class="inp_field">
                            <i class="fas fa-angle-double-right"></i>
                            <input
                                type="text"
                                name="subject"
                                class="subject"
                                id="subject"
                                placeholder="Subject"
                                required />
                        </div>
                        <textarea
                            name="message"
                            cols="30"
                            rows="5"
                            class="message"
                            id="message"
                            placeholder="Message"
                            required></textarea>
                        <button class="submit" id="submit">Submit</button>
                    </form>
                </div>
            </div>
        </div>

        <!-----------------JQUERY {https://jquery.com/} [USED IN portfolio.js]----------------->
        <script src="/resources/js/jquery.min.js"></script>
        <!-----------------MIX IT UP {https://www.kunkalabs.com/mixitup/} [USED IN portfolio.js]----------------->
        <script src="/resources/js/mixitup.min.js"></script>
        <!-----------------SWIPER JS {https://swiperjs.com/} [USED IN portfolio.js, comments.js]----------------->
        <script src="/resources/swiper-js/swiper-bundle.min.js"></script>
        <!-----------------MAPBOX GL {https://www.mapbox.com/} [USED IN contact.js]----------------->
        <script src="/resources/mapbox-gl/mapbox-gl.js"></script>
        <!-----------------EMAIL JS {https://www.emailjs.com/} [USED IN contact.js]----------------->
        <script src="/resources/js/email.min.js"></script>
        <!-----------------ADDITIONAL SCRIPT FOR EMAIL JS----------------->
        <!-----------------VANILLA TILT JS {https://micku7zu.github.io/vanilla-tilt.js/}----------------->
        <script src="/resources/js/vanilla-tilt.min.js"></script>
        <!-----------------ANIME JS {https://animejs.com/} [USED LOCALLY.]----------------->
        <script src="/resources/js/anime.min.js"></script>
        <!-----------------LOCAL (HOME)----------------->
        <script src="/resources/js/home.js"></script>
        <!-----------------LOCAL (ABOUT)----------------->
        <script src="/resources/js/about.js"></script>
        <!-----------------LOCAL (SERVICES)----------------->
        <script src="/resources/js/services.js"></script>
        <!-----------------LOCAL (PORTFOLIO)----------------->
        <script src="/resources/js/portfolio.js"></script>
        <!-----------------LOCAL (COMMENTS)----------------->
        <script src="/resources/js/comments.js"></script>
        <!-----------------LOCAL (MAIN FILE)----------------->
        <script src="/resources/js/main.js"></script>

        <!-----------------CONTACT LOGIC-------------------------->
        <script type="module">
            // The 'building' layer in the mapbox-streets vector source contains building-height
            // data from OpenStreetMap.
            // For more, goto:
            // https://www.mapbox.com/install/

            mapboxgl.accessToken =
                import.meta.env.VITE_MAPBOX_ACCESS_TOKEN || "";
            var map = new mapboxgl.Map({
                style: "mapbox://styles/mapbox/light-v10",
                center: [90.3911645, 23.7494284], // Longitude, latitude
                zoom: 18.5, // Zoom level
                pitch: 45,
                bearing: -17.6,
                container: "map", // Our #map target.
                antialias: true,
            });

            map.on("load", function () {
                // Insert the layer beneath any symbol layer.
                var layers = map.getStyle().layers;

                var labelLayerId;
                for (var i = 0; i < layers.length; i++) {
                    if (
                        layers[i].type === "symbol" &&
                        layers[i].layout["text-field"]
                    ) {
                        labelLayerId = layers[i].id;
                        break;
                    }
                }

                map.addLayer(
                    {
                        id: "3d-buildings",
                        source: "composite",
                        "source-layer": "building",
                        filter: ["==", "extrude", "true"],
                        type: "fill-extrusion",
                        minzoom: 15,
                        paint: {
                            "fill-extrusion-color": "#aaa",

                            // use an 'interpolate' expression to add a smooth transition effect to the
                            // buildings as the user zooms in
                            "fill-extrusion-height": [
                                "interpolate",
                                ["linear"],
                                ["zoom"],
                                15,
                                0,
                                15.05,
                                ["get", "height"],
                            ],
                            "fill-extrusion-base": [
                                "interpolate",
                                ["linear"],
                                ["zoom"],
                                15,
                                0,
                                15.05,
                                ["get", "min_height"],
                            ],
                            "fill-extrusion-opacity": 0.6,
                        },
                    },
                    labelLayerId
                );
            });
            function vanillaTilt(element) {
                VanillaTilt.init(document.querySelector(element), {
                    max: 10,
                    speed: 200,
                    glare: true,
                    "max-glare": 0.5,
                });
            }

            vanillaTilt(".info1");
            vanillaTilt(".info2");
            vanillaTilt(".info3");

            document.querySelector("form").addEventListener("submit", (e) => {
                e.preventDefault();
            });
            let form_name = document.getElementById("fname");
            let email = document.getElementById("email");
            let subject = document.getElementById("subject");
            let message = document.getElementById("message");
            let submit = document.getElementById("submit");

            submit.addEventListener("click", () => {
                if (
                    form_name.value == "" &&
                    email.value == "" &&
                    subject.value == "" &&
                    message.value == ""
                ) {
                    alert("All fields are required");
                    return;
                } else {
                    submitEmail();
                }
            });

            emailjs.init(import.meta.env.VITE_EMAILJS_ACCESS_TOKEN);

            function submitEmail() {
                let param = {
                    method: "POST",
                    from_name: form_name.value,
                    from_email: email.value,
                    to_name: "Shuvro!",
                    subject: subject.value,
                    message: message.value,
                };

                emailjs.send("service_name", "template_name", param).then(
                    function (response) {
                        alert(
                            "SUCCESS! " + response.status + " " + response.text
                        );
                    },
                    function (error) {
                        alert("FAILED... " + error);
                    }
                );
            }

            document.querySelector("form").addEventListener("submit", (e) => {
                e.preventDefault();
            });
        </script>

        <!-----------------LOCAL (MAIN FILE { USED TO ANIMATE WEBPAGE.})----------------->
        <script defer>
            const animate1 = anime.timeline({
                targets: ".circle",
                loop: true,
                duration: 2000,
                direction: "alternate",
                easing: "easeInOutQuad",
            });
            animate1.add({
                translateX: 350,
            });

            let dot = document.querySelectorAll(".dot");
            for (let i = 0; i < dot.length; i++) {
                const ind = dot[i];
                const animate2 = anime.timeline({
                    targets: ind,
                    loop: true,
                    direction: "alternate",
                    delay: i * 100,
                });
                animate2.add({
                    scale: 2,
                });
            }

            let span = document.querySelectorAll(".content .text span");
            const animate3 = anime.timeline({
                targets: span,
                easing: "easeInOutExpo",
                delay: anime.stagger(20, { direction: "reverse" }),
                direction: "reverse",
                autoplay: false,
            });

            animate3.add({
                rotate: () => {
                    return anime.random(-360, 360);
                },
                translateX: () => {
                    return anime.random(-500, 500);
                },
                translateY: () => {
                    return anime.random(-500, 500);
                },
                duration: 3000,
            });

            const animate4 = anime({
                targets: ".button",
                scale: [0, 1],
                delay: anime.stagger(200, { start: 7000 }),
                autoplay: false,
            });

            const animate5 = anime({
                targets: [
                    document.querySelectorAll(".info"),
                    document.querySelectorAll(".inp_field"),
                    ".message",
                    ".submit",
                ],
                translateY: [50, 0],
                rotateX: [90, 0],
                opacity: [0, 1],
                delay: anime.stagger(300, { start: 1000 }),
                duration: 750,
                autoplay: false,
                easing: "easeOutQuint",
            });

            const animate6 = anime({
                targets: [".services .t_dummy", ".services .hero-text"],
                duration: 1000,
                scaleX: [0, 1],
                delay: anime.stagger(300, { start: 1000 }),
                autoplay: false,
            });

            function resize() {
                if (window.innerWidth <= 632) {
                    animate5.play();
                    animate3.play();
                    animate4.play();
                    animate6.play();
                }
            }
            resize();
            window.addEventListener("resize", resize);
        </script>
    </body>
</html>
/* ==================== GOOGLE FONTS ====================*/
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap");

/*==================== VARIABLES CSS ====================*/
:root {
  --header-height: 3rem;

  /*========== Colors ==========*/
  /* Change favorite color */
  --hue-color: 190; /*Purple 250 - Green 142 - Blue 230 - Pink 340*/

  /* HSL color mode */
  --first-color: hsl(var(--hue-color), 69%, 61%);
  --first-color-second: hsl(var(--hue-color), 69%, 61%);
  --first-color-alt: hsl(var(--hue-color), 57%, 53%);
  --first-color-lighter: hsl(var(--hue-color), 92%, 85%);
  --title-color: hsl(var(--hue-color), 8%, 15%);
  --text-color: hsl(var(--hue-color), 8%, 45%);
  --text-color-light: hsl(var(--hue-color), 8%, 65%);
  --input-color: hsl(var(--hue-color), 70%, 96%);
  --body-color: hsl(var(--hue-color), 60%, 99%);
  --container-color: #fff;
  --scroll-bar-color: hsl(var(--hue-color), 12%, 90%);
  --scroll-thumb-color: hsl(var(--hue-color), 12%, 80%);

  /*========== Font and typography ==========*/
  --body-font: "Poppins", sans-serif;

  /* .5rem = 8px, 1rem = 16px, 1.5rem = 24px ... */
  --big-font-size: 2rem;
  --h1-font-size: 1.5rem;
  --h2-font-size: 1.25rem;
  --h3-font-size: 1.125rem;
  --normal-font-size: 0.938rem;
  --small-font-size: 0.813rem;
  --smaller-font-size: 0.75rem;

  /*========== Font weight ==========*/
  --font-medium: 500;
  --font-semi-bold: 600;

  /*========== Margenes Bottom ==========*/
  /* .25rem = 4px, .5rem = 8px, .75rem = 12px ... */
  --mb-0-25: 0.25rem;
  --mb-0-5: 0.5rem;
  --mb-0-75: 0.75rem;
  --mb-1: 1rem;
  --mb-1-5: 1.5rem;
  --mb-2: 2rem;
  --mb-2-5: 2.5rem;
  --mb-3: 3rem;

  /*========== z index ==========*/
  --z-tooltip: 10;
  --z-fixed: 100;
  --z-modal: 1000;
}

/* Font size for large devices */
@media screen and (min-width: 968px) {
  :root {
    --big-font-size: 3rem;
    --h1-font-size: 2.25rem;
    --h2-font-size: 1.5rem;
    --h3-font-size: 1.25rem;
    --normal-font-size: 1rem;
    --small-font-size: 0.875rem;
    --smaller-font-size: 0.813rem;
  }
}

/*========== Variables Dark theme ==========*/
body.dark-theme {
  /* HSL color mode */
  --first-color-second: hsl(var(--hue-color), 30%, 8%);
  --title-color: hsl(var(--hue-color), 8%, 95%);
  --text-color: hsl(var(--hue-color), 8%, 45%);
  --text-color-light: hsl(var(--hue-color), 8%, 75%);
  --input-color: hsl(var(--hue-color), 29%, 16%);
  --body-color: hsl(var(--hue-color), 28%, 12%);
  --container-color: hsl(var(--hue-color), 29%, 16%);
  --scroll-bar-color: hsl(var(--hue-color), 12%, 48%);
  --scroll-thumb-color: hsl(var(--hue-color), 12%, 36%);
}

/*========== Button Dark/Light ==========*/
.nav__btns {
  display: flex;
  align-items: center;
}

.change-theme {
  font-size: 1.25rem;
  color: var(--title-color);
  margin-right: var(--mb-1);
  cursor: pointer;
}

.change-theme:hover {
  color: var(--first-color);
}

/*==================== BASE ====================*/

* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0 0 var(--header-height) 0;
  font-family: var(--body-font);
  font-size: var(--normal-font-size);
  background-color: var(--body-color);
  color: var(--text-color);
}

h1,
h2,
h3,
h4 {
  color: var(--title-color);
  font-weight: var(--font-semi-bold);
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
}

img {
  width: 100%;
  height: auto;
}

/*==================== REUSABLE CSS CLASSES ====================*/
.section {
  padding: 2rem 0 4rem;
  margin-bottom: 40px;
}

.section__title {
  font-size: var(--h1-font-size);
}

.section__subtitle {
  display: block;
  font-size: var(--small-font-size);
  margin-bottom: var(--mb-2);
}

.section__title,
.section__subtitle {
  text-align: center;
}

/*==================== LAYOUT ====================*/

.container {
  max-width: 768px;
  margin-left: var(--mb-1-5);
  margin-right: var(--mb-1-5);
}

.grid {
  display: grid;
  gap: 1.5rem;
}

.header {
  width: 100%;
  position: fixed;
  bottom: 0;
  left: 0;
  z-index: var(--z-fixed);
  background-color: var(--body-color);
}

/*==================== NAV ====================*/
.nav {
  max-width: 968px;
  height: var(--header-height);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.nav__logo,
.nav__toggle {
  color: var(--title-color);
  font-weight: var(--font-medium);
}

.nav__logo:hover {
  color: var(--first-color);
}

.nav__toggle {
  font-size: 1.1rem;
  cursor: pointer;
}

.nav__toggle:hover {
  color: var(--first-color);
}

@media screen and (max-width: 767px) {
  .nav__menu {
    position: fixed;
    bottom: -100%;
    left: 0;
    width: 100%;
    background-color: var(--body-color);
    padding: 2rem 1.5rem 4rem;
    box-shadow: 0 -1px 4px rgba(0, 0, 0, 0.15);
    border-radius: 1.5rem 1.5rem 0 0;
    transition: 0.3s;
  }
}

.nav__list {
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
}
.nav__link {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-size: var(--small-font-size);
  color: var(--title-color);
  font-weight: var(--font-medium);
}

.nav__link:hover {
  color: var(--first-color);
}

.nav__icon {
  font-size: 1.2rem;
}

.nav__close {
  position: absolute;
  right: 1.3rem;
  bottom: 0.5rem;
  font-size: 1.5rem;
  cursor: pointer;
  color: var(--first-color);
}

.nav__close:hover {
  color: var(--first-color-alt);
}

/* show menu */
.show-menu {
  bottom: 0;
}

/* Active link */
.active-link {
  color: var(--first-color);
}

/* Change background header */
.scroll-header {
  box-shadow: 0 -1px 4px rgba(0, 0, 0, 0.15);
}

/*==================== HOME ====================*/

.home__container {
  gap: 1rem;
}

.home__content {
  grid-template-columns: 0.5fr 3fr;
  padding-top: 3.5rem;
  align-items: center;
}

.home__social {
  display: grid;
  grid-template-columns: max-content;
  row-gap: 1rem;
}

.home__social-icon {
  font-size: 1.25rem;
  color: var(--first-color);
}

.home__social-icon:hover {
  color: var(--first-color-alt);
}

.home__blob {
  width: 200px;
  fill: var(--first-color);
}

.home__blob-img {
  width: 220px;
}

.home__data {
  grid-column: 1/3;
}

.home__title {
  font-size: var(--big-font-size);
}

.home__subtitle {
  font-size: var(--h3-font-size);
  color: var(--text-color);
  font-weight: var(--font-medium);
  margin-bottom: var(--mb-0-75);
}

.home__description {
  margin-bottom: var(--mb-2);
}

.home__scroll {
  display: none;
}

.home__scroll-button {
  color: var(--first-color);
  transition: 0.3s;
}

.home__scroll-button:hover {
  transform: translateY(0.25rem);
}

.home__scroll-mouse {
  font-size: 2rem;
}

.home__scroll-name {
  font-size: var(--small-font-size);
  color: var(--title-color);
  font-weight: var(--font-medium);
  margin-right: var(--mb-0-25);
}

.home__scroll-arrow {
  font-size: 1.25rem;
}
/*==================== BUTTONS ====================*/

.button {
  display: inline-block;
  background-color: var(--first-color);
  color: #ffff;
  padding: 1rem;
  border-radius: 0.5rem;
  font-weight: var(--font-medium);
}

.button:hover {
  background-color: var(--first-color-alt);
}

.button__icon {
  font-size: 1.2rem;
  margin-left: var(--mb-0-5);
  transition: 0.3s;
}

.button--white {
  background-color: #fff;
  color: var(--first-color);
}

.button--white:hover {
  background-color: #fff;
}

.button--flex {
  display: inline-flex;
  align-items: center;
  transition: 0.3s;
}

.button--small {
  padding: 0.75rem 1rem;
}

.button--link {
  padding: 0;
  background-color: transparent;
  color: var(--first-color);
}

.button--link:hover {
  background-color: transparent;
  color: var(--first-color-alt);
}

/*==================== ABOUT ====================*/
.about__img {
  width: 200px;
  border-radius: 0.5rem;
  justify-self: center;
  align-items: center;
}

.about__description {
  text-align: center;
  margin-bottom: var(--mb-2-5);
}

.about__info {
  display: flex;
  justify-content: space-evenly;
  margin-bottom: var(--mb-2-5);
}

.about__info-title {
  font-size: var(--h2-font-size);
  font-weight: var(--font-semi-bold);
  color: var(--title-color);
}

.about__info-name {
  font-size: var(--smaller-font-size);
}

.about__info-title,
.about__info-name {
  display: block;
  text-align: center;
}

.about__buttons {
  display: flex;
  justify-content: center;
}

/*==================== SKILLS ====================*/

.skills__container {
  row-gap: 0;
}

.skills__header {
  display: flex;
  align-items: center;
  margin-bottom: var(--mb-2-5);
  cursor: pointer;
}

.skills__icon,
.skills__arrow {
  font-size: 2rem;
  color: var(--first-color);
}

.skills__icon {
  margin-right: var(--mb-0-75);
}

.skills__title {
  font-size: var(--h3-font-size);
}

.skills__subtitle {
  font-size: var(--small-font-size);
  color: var(--text-color-light);
}

.skills__arrow {
  margin-left: auto;
  transition: 0.4s;
}

.skills__list {
  row-gap: 1.5rem;
  padding-left: 2.7rem;
}

.skills__titles {
  display: flex;
  justify-content: space-between;
  margin-bottom: var(--mb-0-5);
}

.skills__name {
  font-size: var(--normal-font-size);
  font-weight: var(--font-medium);
}

.skills__bar,
.skills__percentage {
  height: 5px;
  border-radius: 0.25rem;
}

.skills__bar {
  background-color: var(--first-color-lighter);
}

.skills__percentage {
  display: block;
  background-color: var(--first-color);
}

.skills__html {
  width: 90%;
}

.skills__css {
  width: 80%;
}

.skills__js {
  width: 60%;
}

.skills__wordpress {
  width: 70%;
}

.skills__python {
  width: 60%;
}

.skills__tab {
  width: 70%;
}

.skills__sql {
  width: 50%;
}

.skills__google {
  width: 70%;
}

.skills__bank {
  width: 80%;
}

.skills__google {
  width: 70%;
}

.skills__counter {
  width: 80%;
}

.skills__office {
  width: 90%;
}

.skills__close .skills__list {
  height: 0;
  overflow: hidden;
}

.skills__open .skills__list {
  height: max-content;
  margin-bottom: var(--mb-2-5);
}

.skills__open .skills__arrow {
  transform: rotate(-180deg);
}

/*==================== QUALIFICATION ====================*/
.qualification__tabs {
  display: flex;
  justify-content: space-evenly;
  margin-bottom: var(--mb-2);
}

.qualification__button {
  font-size: var(--h3-font-size);
  font-weight: var(--font-medium);
  cursor: pointer;
}

.qualification__button:hover {
  color: var(--first-color);
}

.qualification__icon {
  font-size: 1.8rem;
  margin-right: var(--mb-0-25);
}

.qualification__data {
  display: grid;
  grid-template-columns: 1fr max-content 1fr;
  column-gap: 1.5rem;
}

.qualification__title {
  font-size: var(--normal-font-size);
  font-weight: var(--font-medium);
}

.qualification__subtitle {
  display: inline-block;
  font-size: var(--small-font-size);
  margin-bottom: var(--mb-1);
}

.qualification__calendar {
  font-size: var(--smaller-font-size);
  color: var(--text-color-light);
  /* margin-bottom: var(--mb-1) */
}

.qualification__rounder {
  display: inline-block;
  width: 13px;
  height: 13px;
  background-color: var(--first-color);
  border-radius: 50%;
}

.qualification__line {
  display: block;
  width: 1px;
  height: 100%;
  background-color: var(--first-color);
  transform: translate(6px, -7px);
}

.qualification__content[data-content] {
  display: none;
}

.qualification__active[data-content] {
  display: block;
}

.qualification__button.qualification__active {
  color: var(--first-color);
}

/*==================== SERVICES ====================*/
.services__container {
  gap: 1.5rem;
  grid-template-columns: repeat(2, 1fr);
}

.services__content {
  position: relative;
  background-color: var(--container-color);
  padding: 3.5rem 0.5rem 1.25rem 1.5rem;
  border-radius: 0.25rem;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.15);
  transition: 0.3s;
}

.services__content:hover {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
}

.services__icon {
  display: block;
  font-size: 1.5rem;
  color: var(--first-color);
  margin-bottom: var(--mb-1);
}

.services__title {
  font-size: var(--h3-font-size);
  margin-bottom: var(--mb-1);
  font-weight: var(--font-medium);
}

.services__button {
  cursor: pointer;
  font-size: var(--small-font-size);
}

.services__button:hover .button__icon {
  transform: translateX(0.25rem);
}

.services__modal {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0 1rem;
  z-index: var(--z-modal);
  opacity: 0;
  visibility: hidden;
  transition: 0.3s;
}

.services__modal-content {
  position: relative;
  background-color: var(--container-color);
  padding: 1.5rem;
  border-radius: 0.5rem;
}

.services__modal-services {
  row-gap: 1rem;
}

.services__modal-service {
  display: flex;
}

.services__modal-title {
  font-size: var(--h3-font-size);
  font-weight: var(--font-medium);
  margin-bottom: var(--mb-1-5);
}

.services__modal-close {
  position: absolute;
  top: 1rem;
  right: 1rem;
  font-size: 1.5rem;
  color: var(--first-color);
  cursor: pointer;
}

.services__modal-icon {
  color: var(--first-color);
  margin-right: var(--mb-0-25);
}

/* Active Modal */
.active-modal {
  opacity: 1;
  visibility: visible;
}

/*==================== PORTFOLIO ====================*/
.portfolio__container {
  overflow: initial;
}

.portfolio__content {
  padding: 0 1.5rem;
}

.portfolio__img {
  width: 265px;
  border-radius: 0.5rem;
  justify-self: center;
}

.portfolio__title {
  font-size: var(--h3-font-size);
  margin-bottom: var(--mb-0-5);
}

.portfolio__description {
  margin-bottom: var(--mb-0-75);
}

.portfolio__button:hover .button__icon {
  transform: translateX(0.25rem);
}

.swiper-button-prev::after,
.swiper-button-next::after {
  content: "";
}

.swiper-portfolio-icon {
  font-size: 2rem;
  color: var(--first-color);
}

.swiper-button-prev {
  left: -0.5rem;
}

.swiper-button-next {
  right: -0.5rem;
}

.swiper-container-horizontal > .swiper-pagination-bullets {
  bottom: -2.5rem;
}

.swiper-pagination-bullet-active {
  background-color: var(--first-color);
}

.swiper-button-prev,
.swiper-button-next,
.swiper-pagination-bullet {
  outline: none;
}
/*==================== PROJECT IN MIND ====================*/
.project {
  text-align: center;
}

.project__bg {
  background-color: var(--first-color-second);
  padding-top: 3rem;
}

.project__title {
  font-size: var(--h2-font-size);
  margin-bottom: var(--mb-0-75);
}

.project__description {
  margin-bottom: var(--mb-1-5);
}

.project__title,
.project__description {
  color: #fff;
}

.project__img {
  width: 232px;
  justify-self: center;
}

/*==================== TESTIMONIAL ====================*/
.testimonial__data,
.testimonial__header {
  display: flex;
}

.testimonial__data {
  justify-content: space-between;
  margin-bottom: var(--mb-1);
}

.testimonial__img {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  margin-right: var(--mb-0-75);
}

.testimonial__name {
  font-size: var(--h3-font-size);
  font-weight: var(--font-medium);
}

.testimonial__client {
  font-size: var(--small-font-size);
  color: var(--text-color-light);
}

.testimonial__description {
  margin-bottom: var(--mb-2-5);
}

.testimonial__icon-star {
  color: var(--first-color);
}

.swiper-container .swiper-pagination-testimonial {
  bottom: 0;
}

/*==================== CONTACT ME ====================*/
.contact__container {
  row-gap: 3rem;
}

.contact__information {
  display: flex;
  margin-bottom: var(--mb-2);
}

.contact__icon {
  font-size: 1.5rem;
  color: var(--first-color);
  margin-right: var(--mb-0-75);
}

.content__title {
  font-size: var(--h3-font-size);
  font-weight: var(--font-medium);
}

.contact__subtitle {
  font-size: var(--small-font-size);
  color: var(--text-color-light);
}

.contact__content {
  background-color: var(--input-color);
  border-radius: 0.5rem;
  padding: 0.75rem 1rem 0.25rem;
}

.contact__label {
  font-size: var(--smaller-font-size);
  color: var(--title-color);
}

.contact__input {
  width: 100%;
  background-color: var(--input-color);
  color: var(--text-color);
  font-family: var(--body-font);
  font-size: var(--normal-font-size);
  border: none;
  outline: none;
  padding: 0.25rem 0.5rem 0.5rem 0;
}

/*==================== FOOTER ====================*/
.footer {
  padding-top: 2rem;
}

.footer__container {
  row-gap: 3.5rem;
}

.footer__bg {
  background-color: var(--first-color-second);
  padding: 2rem 0 3rem;
}

.footer__title {
  font-size: var(--h1-font-size);
  margin-bottom: var(--mb-0-25);
}

.footer__subtitle {
  font-size: var(--small-font-size);
}

.footer__links {
  display: flex;
  flex-direction: column;
  row-gap: 1.5rem;
}

.footer__link:hover {
  color: var(--first-color-lighter);
}

.footer__social {
  font-size: 1.25rem;
  margin-right: var(--mb-1-5);
}

.footer__social:hover {
  color: var(--first-color-lighter);
}

.footer__copy {
  font-size: var(--smaller-font-size);
  text-align: center;
  color: var(--text-color-light);
  margin-top: var(--mb-3);
}

.footer__title,
.footer__subtitle,
.footer__link,
.footer__social {
  color: #fff;
}

/*========== SCROLL UP ==========*/
.scrollup {
  position: fixed;
  right: 1rem;
  bottom: -20%;
  background-color: var(--first-color);
  opacity: 0.8;
  padding: 0 0.3rem;
  border-radius: 0.4rem;
  z-index: var(--z-tooltip);
  transition: 0.4s;
}

.scrollup:hover {
  background-color: var(--first-color-alt);
}

.scrollup__icon {
  font-size: 1.5rem;
  color: #fff;
}

/* Show scroll */
.show-scroll {
  bottom: 5rem;
}

/*========== SCROLL BAR ==========*/
::-webkit-scrollbar {
  width: 0.6rem;
  background-color: var(--scroll-bar-color);
  border-radius: 0.5rem;
}

::-webkit-scrollbar-thumb {
  background-color: var(--scroll-thumb-color);
  border-radius: 0.5rem;
}

::-webkit-scrollbar-thumb:hover {
  background-color: var(--text-color-light);
}

/*==================== MEDIA QUERIES ====================*/
/* For small devices */
@media screen and (max-width: 380px) {
  .container {
    margin-left: var(--mb-1);
    margin-right: var(--mb-1);
  }

  .nav__menu {
    padding: 2rem 0.25rem 4rem;
  }

  .nav__list {
    column-gap: 0;
  }

  .home__content {
    grid-template-columns: 0.35fr 3fr;
  }

  .home__blob {
    width: 250px;
  }

  .home__social-icon {
    width: 30px;
  }

  .home__subtitle {
    font-size: 24px;
  }

  .home__description {
    font-size: 18px;
  }

  .home__button {
    font-size: 20px;
  }

  .skills__title {
    font-size: var(--normal-font-size);
  }
  .qualification__data {
    gap: 0.5rem;
  }

  .services__container {
    grid-template-columns: max-content;
    justify-content: center;
  }

  .services__content {
    padding-right: 3.5rem;
  }
  .services__modal {
    padding: 0 0.5rem;
  }

  .project__img {
    width: 200px;
  }

  .testimonial__header,
  .testimonial__data {
    flex-direction: column;
    align-items: center;
  }

  .testimonial__img {
    margin-right: 0;
    margin-bottom: var(--mb-0-25);
  }

  .testimonial__data,
  .testimonial__description {
    text-align: center;
  }
}

/* For medium devices */
@media screen and (min-width: 568px) {
  .home__content {
    grid-template-columns: max-content 1fr 1fr;
  }

  .home__data {
    grid-column: initial;
  }
  .home__img {
    order: 1;
    justify-self: center;
  }

  .about__container,
  .skills_container,
  .portfolio__content,
  .project__container,
  .contact__container,
  .footer__container {
    grid-template-columns: repeat(2, 1fr);
  }

  .qualification__sections {
    display: grid;
    grid-template-columns: 0.6fr;
    justify-content: center;
  }

  @media screen and (min-width: 768px) {
    .container {
      margin-left: auto;
      margin-right: auto;
    }

    .body {
      margin: 0;
    }
    .section {
      padding: 6rem 0 2rem;
    }
    .section__subtitle {
      margin-bottom: 4rem;
    }
    .header {
      top: 0;
      bottom: initial;
    }

    .header,
    .main,
    .footer__container {
      padding: 0 1rem;
    }

    .nav {
      height: calc(var(--header-height) + 1.5rem);
      column-gap: 1rem;
    }
    .nav__icon,
    .nav__close,
    .nav__toggle {
      display: none;
    }

    .nav__list {
      display: flex;
      column-gap: 2rem;
    }

    .nav__menu {
      margin-left: auto;
    }
    .change-theme {
      margin: 0;
    }

    .home__container {
      row-gap: 5rem;
    }

    .home__content {
      padding-top: 5.5rem;
      column-gap: 2rem;
    }
    .home__blob {
      width: 270px;
    }
    .home__scroll {
      display: block;
    }
    .home__scroll-button {
      margin-left: 3rem;
    }
    .about__container {
      column-gap: 5rem;
    }
    .about__img {
      width: 350px;
    }
    .about__description {
      text-align: initial;
    }
    .about__info {
      justify-content: space-between;
    }
    .about__buttons {
      justify-content: initial;
    }
    .qualification__tabs {
      justify-content: center;
    }
    .qualification__button {
      margin: 0 var(--mb-1);
    }

    .qualification__sections {
      grid-template-columns: 0.5fr;
    }
    .services__container {
      grid-template-columns: repeat(3, 218px);
      justify-content: center;
    }
    .services__icon {
      font-size: 2rem;
    }
    .services__content {
      padding: 6rem 0 2rem 2.5rem;
    }

    .services__modal-content {
      width: 450px;
    }
    .portfolio__img {
      width: 320px;
    }
    .portfolio__content {
      align-items: center;
    }
    .project {
      text-align: initial;
    }
    .project__bg {
      background: none;
    }
    .project__container {
      background-color: var(--first-color-second);
      border-radius: 1rem;
      padding: 3rem 2.5rem 0;
      grid-template-columns: 1fr max-content;
      column-gap: 3rem;
    }
    .project__data {
      padding-top: 0.8rem;
    }
    .footer__container {
      grid-template-columns: repeat(3, 1fr);
    }
    .footer__bg {
      padding: 3rem 0 3.5rem;
    }

    .footer__links {
      flex-direction: row;
      column-gap: 2rem;
    }
    .footer__socials {
      justify-self: flex-end;
    }
    .footer__copy {
      margin-top: 4.5rem;
    }
  }
}

/* For large devices */
@media screen and (min-width: 1024px) {
  body {
    margin: 0;
  }

  .header,
  .main,
  .footer__container {
    padding: 0;
  }
  .home__blob {
    width: 320px;
  }
  .home__social {
    transform: translateX(-6rem);
  }
  .services__container {
    grid-template-columns: repeat(3, 238px);
  }
  .portfolio__content {
    column-gap: 5rem;
  }

  .project__container {
    padding-bottom: 30px;
  }

  .swiper-portfolio-icon {
    font-size: 3.5rem;
  }
  .swiper-button-prev {
    left: -3.5rem;
  }
  .swiper-button-next {
    right: -3.5rem;
  }
  .swiper-container-horizontal > .swiper-pagination-bullets {
    bottom: -4.5rem;
  }

  .contact__form {
    width: 460px;
  }
  .contact__inputs {
    grid-template-columns: repeat(2, 1fr);
  }
}
