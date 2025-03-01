@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap");

/*================ VARIABLES CSS ==========*/

:root {
  --header-height: 3rem;

  /*======= Colors =======*/
  /* Change Favorite color */
  --hue-color: 240;

  /*========= HSL Color mode =========*/
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

  /*========= Font and typography ===========*/
  --body-font: "Poppins", sans-serif;

  --big-font-size: 2rem;
  --h1-font-size: 1.5rem;
  --h2-font-size: 1.25rem;
  --h3-font-size: 1.125rem;
  --normal-font-size: 0.938rem;
  --small-font-size: 0.813rem;
  --smaller-font-size: 0.75rem;

  /*=========== Font weight ==========*/

  --font-medium: 500;
  --font-semi-bold: 600;

  /*============ Margin Bottom ===========*/
  /* .25rem = 4px, .5rem=8px, .75rem = 12px*/
  --mb-0-25: 0.25rem;
  --mb-0-5: 0.5rem;
  --mb-0-75: 0.75rem;
  --mb-1: 1rem;
  --mb-1-5: 1.5rem;
  --mb-2: 2rem;
  --mb-2-5: 2.5rem;
  --mb-3: 3rem;

  /*============== z index =============*/
  --z-tooltip: 10;
  --z-fixed: 100;
  --z-modal: 1000;
}

/* Font Size for larger devices */
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
/*================= Variables Dark Theme ===============*/
body.dark-theme {
  /*========= HSL Color mode =========*/

  --first-color-second: hsl(var(--hue-color), 30%, 8%);
  --title-color: hsl(var(--hue-color), 8%, 95%);
  --text-color: hsl(var(--hue-color), 8%, 75%);
  --input-color: hsl(var(--hue-color), 29%, 16%);
  --body-color: hsl(var(--hue-color), 28%, 12%);
  --container-color: hsl(var(--hue-color), 29%, 16%);
  --scroll-bar-color: hsl(var(--hue-color), 12%, 48%);
  --scroll-thumb-color: hsl(var(--hue-color), 12%, 36%);
}

/*================= Button Dark/Light ===============*/
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

/*================= Base ===============*/
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
  max-width: 100%;
  height: auto;
}
.section {
  padding: 2rem 0 4rem;
}
.section__title {
  font-size: var(--h1-font-size);
}

.section__subtitle {
  display: block;
  font-size: var(--small-font-size);
  margin-bottom: var(--mb-3);
}
.section__title,
.section__subtitle {
  text-align: center;
}

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

/* Show Menu */
.show-menu {
  bottom: 0;
}

/* Active Link */
.active-link {
  color: var(--first-color);
}

/* Change Background header */
.scroll-header {
  box-shadow: 0 -1px 4px rgba(0, 0, 0, 0.15);
}

/*========HOME=============*/
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
  font-size: 1.05rem;
  color: var(--first-color);
}
.home__social-icon:hover {
  color: var(--first-color-lighter);
}

.home__blob {
  width: 200px;
  fill: var(--first-color);
  /* fill: hsl(69, 69%, 61%); */
}
.home__blob-img {
  width: 180%;
  height: 145%;
  padding-left: 30px;
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

.portfolio__scroll {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 15px;
  cursor: pointer;
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

/*================== Buttons ===================*/
.button {
  display: inline-block;
  background-color: var(--first-color);
  color: #fff;
  padding: 1rem;
  margin-bottom: 10px;
  border-radius: 0.5rem;
  font-weight: var(--font-medium);
}

.button:hover {
  background-color: var(--first-color-alt);
}

.button__icon {
  font-size: 1.25rem;
  margin-left: 0.25rem;
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

/*===================== About ==================*/
.about__img {
  width: 170px;
  border-radius: 500%;
  justify-self: center;
  align-self: center;
  /* border: 1px solid #fff; */
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

.about__info-name,
.about__info-title {
  display: block;
  text-align: center;
}

.about__buttons {
  display: flex;
  justify-content: center;
}

/*===================== SKILLS =========================*/

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
  font-size: 1.25rem;
  color: var(--first-color);
}

.skills__icon {
  margin-right: var(--mb-0-75);
}

.skills__title {
  font-size: var(--h3-font-size);
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
  width: 55%;
}
.skills__react {
  width: 40%;
}

.skills__php {
  width: 80%;
}
.skills__node {
  width: 70%;
}
.skills__firebase {
  width: 75%;
}
.skills__python {
  width: 50%;
}

.skills__figma {
  width: 85%;
}
.skills__sketch {
  width: 75%;
}
.skills__photoshop {
  width: 60%;
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

/*==================== Qualifications ====================*/

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
}

.qualification__calender {
  font-size: var(--smaller-font-size);
  color: var(--text-color-light);
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

.qualification [data-content] {
  display: none;
}

.qualification__active[data-content] {
  display: none;
}

.qualification__button.qualification__active {
  color: var(--first-color);
}

/*================= Services ==================*/

.services_container {
  gap: 1.5rem;
  grid-template-columns: repeat(2, 1fr);
}

.services__content {
  position: relative;
  background-color: var(--container-color);
  padding: 3.5rem 0.5rem 1.25rem 1.5rem;
  border-radius: 0.25rem;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.15);
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
  border-radius: 1.25rem;
}
.services__modal-services {
  row-gap: 1rem;
}

.services__modal-service {
  display: flex;
}
.services__modal-title {
  font-size: var(--h3-font-size);
  font-family: var(--font-medium);
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

/*================== Portfolio ==================*/

.portfolio__container {
  overflow: initial;
}
/*need change*/
.portfolio__content {
  padding: 0 1.5rem;
}
.portfolio__img {
  width: 310px;
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
.swiper-pagination-bullets-active {
  background-color: var(--first-color);
}

.swiper-button-next,
.swiper-button-prev,
.swiper-pagination-bullets {
  outline: none;
}

/*================ Contact Me ===============*/

.contact__container {
  row-gap: 2rem;
}

.contact__information {
  display: flex;
  margin-bottom: var(--mb-2);
}

.contact__icon {
  font-size: 2rem;
  color: var(--first-color);
  margin-right: var(--mb-0-75);
}

.contact__title {
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

/*=================== Footer ==================*/

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
  transition: 0.3s;
}

.footer__social {
  font-size: 1.25rem;
  margin-right: var(--mb-1-5);
}

.footer__social:hover {
  color: var(--first-color-lighter);
  transition: 0.3s;
}

.footer__copy {
  font-size: var(--smaller-font-size);
  text-align: center;
  color: var(--text-color-light);
  margin-top: var(--mb-3);
}

.footer__title,
.footer__link,
.footer__subtitle,
.footer__social {
  color: #fff;
}

/*==================== Scroll Up ==================*/

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

/* Show Scroll */
.show-scroll {
  bottom: 5rem;
}

/*====================== Scroll Bar =====================*/

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

/*======================== Media Queries ======================*/

/* For Small Devices */
@media screen and (max-width: 350px) {
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
    grid-template-columns: 0.25fr 3fr;
  }

  .home__blob {
    width: 180px;
  }

  .skills__icon,
  .skills__arrow {
    font-size: 1.25rem;
  }
  .skills__title {
    font-size: var(--normal-font-size);
  }

  .qualification__data {
    gap: 0.5rem;
  }

  .services__container {
    justify-content: center;
  }

  .services__content {
    padding-right: 0.5rem;
  }

  .services__modal {
    padding: 0 0.5rem;
  }

  .project__img {
    width: 200px;
  }
}

/* For medium Devices */
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
  .skills__container,
  .project__container,
  .contact__container,
  .footer__container {
    grid-template-columns: repeat(2, 1fr);
  }

  .qualification__section {
    display: grid;
    grid-template-columns: 0.6fr;
    justify-content: center;
  }
}

@media screen and (min-width: 768px) {
  .container {
    margin-left: auto;
    margin-right: auto;
  }

  body {
    margin: 0;
  }

  .section {
    padding: 6rem 0 4rem;
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
    width: 240px;
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
    width: 300px;
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

  .skills__icon,
  .skills__arrow {
    font-size: 1.75rem;
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
  .services_container {
    grid-template-columns: repeat(3, 218px);
    justify-content: center;
  }
  .services__content {
    padding: 6rem 0 2rem 2.5rem;
  }
  .services__icon {
    font-size: 2rem;
  }
  .services__modal-content {
    width: 500px;
  }
  .testimonials {
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

/* For large devices */

@media screen and (min-width: 968px) {
  .header,
  .main,
  .footer__container {
    padding: 0;
  }

  .home__blob {
    width: 280px;
  }

  .home__title {
    font-size: 37px;
  }

  .home__social {
    transform: translateX(-6rem);
  }

  .button--white {
    bottom: -4.5rem;
  }
}
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Portfolio</title>
    <link rel="stylesheet" href="assets/swiper-bundle.min.css" />
    <link rel="stylesheet" href="assets/newcss.css" />
    <link
      rel="stylesheet"
      href="https://unicons.iconscout.com/release/v4.0.8/css/line.css"
    />
  </head>

  <body oncontextmenu="return false">
    <header class="header" id="header">
      <nav class="nav container">
        <a href="#" class="nav__logo">Venkatesh</a>
        <div class="nav__menu" id="nav-menu">
          <ul class="nav__list grid">
            <li class="nav__item">
              <a href="#home" class="nav__link active-link">
                <i class="uil uil-estate nav__icon"></i>Home
              </a>
            </li>
            <li class="nav__item">
              <a href="#about" class="nav__link">
                <i class="uil uil-user nav__icon"></i>About
              </a>
            </li>
            <li class="nav__item">
              <a href="#skills" class="nav__link">
                <i class="uil uil-file-alt nav__icon"></i>Skills
              </a>
            </li>
            <li class="nav__item">
              <a href="#qualification" class="nav__link">
                <i class="uil uil-briefcase-alt nav__icon"></i>Qualification
              </a>
            </li>
            <li class="nav__item">
              <a href="#portfolio" class="nav__link">
                <i class="uil uil-scenery nav__icon"></i>Projects
              </a>
            </li>
            <li class="nav__item">
              <a href="#contact" class="nav__link">
                <i class="uil uil-message nav__icon"></i>Contact-Me
              </a>
            </li>
          </ul>
          <i class="uil uil-times nav__close" id="nav-close"></i>
        </div>
        <div class="nav__btns">
          <!-- Theme change button -->
          <i class="uil uil-moon change-theme" id="theme-button"></i>

          <div class="nav__toggle" id="nav-toggle">
            <i class="uil uil-apps"></i>
          </div>
        </div>
      </nav>
    </header>
    <!-- main-->

    <main class="main">
      <!--========================= Home =====================-->

      <section class="home section" id="home">
        <div class="home__container container grid">
          <div class="home__content grid">
            <div class="home__social">
              <a
                href="https://www.linkedin.com/in/venkateeshh/"
                target="_blank"
                class="home__social-icon"
              >
                <i class="uil uil-linkedin-alt home__icon"></i>
              </a>

              <a
                href="https://github.com/Venkateeshh"
                target="_blank"
                class="home__social-icon"
              >
                <i class="uil uil-github-alt home__icon"></i>
              </a>
            </div>
            <div class="home__img">
              <svg
                class="home__blob"
                viewBox="0 0 200 187"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
              >
                <mask id="mask0" mask-type="alpha">
                  <path
                    d="M190.312 36.4879C206.582 62.1187 201.309 102.826 182.328 134.186C163.346 165.547 
                      130.807 187.559 100.226 186.353C69.6454 185.297 41.0228 161.023 21.7403 129.362C2.45775 
                      97.8511 -7.48481 59.1033 6.67581 34.5279C20.9871 10.1032 59.7028 -0.149132 97.9666 
                      0.00163737C136.23 0.303176 174.193 10.857 190.312 36.4879Z"
                  />
                </mask>
                <g mask="url(#mask0)">
                  <path
                    d="M190.312 36.4879C206.582 62.1187 201.309 102.826 182.328 134.186C163.346 
                      165.547 130.807 187.559 100.226 186.353C69.6454 185.297 41.0228 161.023 21.7403 
                      129.362C2.45775 97.8511 -7.48481 59.1033 6.67581 34.5279C20.9871 10.1032 59.7028 
                     -0.149132 97.9666 0.00163737C136.23 0.303176 174.193 10.857 190.312 36.4879Z"
                  />
                  <image
                    class="home__blob-img"
                    x="-79"
                    y="-46"
                    xlink:href="assets/img/Pro.jpg"
                  />
                </g>
              </svg>
            </div>
            <div class="home__data">
              <h1 class="home__title">Hi, I'm Venkatesh Kamath</h1>
              <h3 class="home__subtitle">
                Information Science Engineering Student
              </h3>
              <p class="home__description">
                A third-year undergraduate engineering student at
                <strong>Canara Engineering College </strong>, Manglore.
              </p>
              <a href="#contact" class="button button--flex">
                Contact me<i class="uil uil-message button__icon"></i>
              </a>
            </div>
          </div>

          <div class="home__scroll">
            <a href="#about" class="home__scroll-button button--flex">
              <i class="uil uil-mouse-alt home__scroll-mouse"></i>
              <span class="home__scroll-name">Scroll down</span>
              <i class="uil uil-arrow-down home__scroll-arrow"></i>
            </a>
          </div>
        </div>
      </section>

      <!--======================= About========================-->

      <section class="about section" id="about">
        <h2 class="section__title">About Me</h2>
        <span class="section__subtitle">My introduction</span>

        <div class="about__container container grid">
          <img src="assets\img\about.jpg" alt="" class="about__img" />

          <div class="about__data">
            <p class="about__description">
              I'm a third-year ISE undergraduate, passionate about technology and an avid reader. I have a self-motivated and can-do attitude, thriving in challenging and dynamic environments. Seeking a competitive position to enhance my skills and contribute to a professional organization. I'm very much passionate to learn new stuff that interests me and can help me to get better.
            </p>

            <div class="about__info">
              <div>
                <span class="about__info-title">08.30+</span>
                <span class="about__info-name">Aggregate <br />CGPA</span>
              </div>

              <div>
                <span class="about__info-title">04+</span>
                <span class="about__info-name"
                  >
                  Projects</span
                >
              </div>

              <div>
                <span class="about__info-title">01+</span>
                <span class="about__info-name">Months <br />experience</span>
              </div>
            </div>

            <div class="about__buttons">
              <a download="" href="assets\MyCV.pdf" class="button button--flex">
                Download CV<i class="fas fa-download button__icon"></i>
              </a>
            </div>
          </div>
        </div>
      </section>

      <!--===================== SKILLS =====================-->

      <section class="skills section" id="skills">
        <h2 class="section__title">Skills</h2>
        <span class="section__subtitle">My technical level</span>

        <div class="skills__container container grid">
          <div>
            <!--==================== Skill 1 =================-->
            <div class="skills__content skills__open">
              <div class="skills__header">
                <i class="fas fa-pencil-ruler skills__icon"></i>

                <div>
                  <h1 class="skills__title">Programming Languages</h1>
                </div>

                <i class="uil uil-angle-down skills__arrow"></i>
              </div>
              

              <div class="skills__list grid">
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">C</h3>
                  </div>
                  
                </div>
                
                  <div class="skills__data">
                    <div class="skills__titles">
                      <h3 class="skills__name">Java</h3>
                    </div>
                    
                  </div>
                  <div class="skills__data">
                    <div class="skills__titles">
                      <h3 class="skills__name">JavaScript</h3>
                    </div>
                    
                  </div>
                  <div class="skills__data">
                    <div class="skills__titles">
                      <h3 class="skills__name">Python</h3>
                    </div>
                   
                  </div>
                  <div class="skills__data">
                    <div class="skills__titles">
                      <h3 class="skills__name">TypeScript</h3>
                    </div>
                </div>
                
                
              </div>
            </div>

            <!--==================== Skill 2 =================-->
            <div class="skills__content skills__close">
              <div class="skills__header">
                <i class="fas fa-code skills__icon"></i>

                <div>
                  <h1 class="skills__title">IT Constructs</h1>
                </div>

                <i class="uil uil-angle-down skills__arrow"></i>
              </div>

              <div class="skills__list grid">
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">DBMS</h3>
                  </div>
                  
                </div>
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">DS & Algorithms</h3>
                  </div>
                  
                </div>
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">OOP</h3>
                  </div>
                  
                </div>
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">OS</h3>
                  </div>
                  
                </div>
                
              </div>
            </div>
          </div>

          <div>
            <!--==================== Skill 3 =================-->
            <div class="skills__content skills__close">
              <div class="skills__header">
                <i class="fas fa-swatchbook skills__icon"></i>
                <div>
                  <h1 class="skills__title">Technologies</h1>
                </div>

                <i class="uil uil-angle-down skills__arrow"></i>
              </div>

              <div class="skills__list grid">
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">Git</h3>
                  </div>
                  
                </div>
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">MongoDB</h3>
                  </div>
                  
                </div>
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">MySQL</h3>
                  </div>
                  
                </div>
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">NextJs</h3>
                  </div>
                  
                </div>
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">NodeJs</h3>
                  </div>
                  
                </div>
                
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">Tailwind</h3>
                  </div>
                  
                </div>
                <div class="skills__data">
                  <div class="skills__titles">
                    <h3 class="skills__name">MySQL</h3>
                  </div>
                  
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!--==================== Qualifications ==================-->

      <section
        class="qualification__section service__section"
        id="qualification"
      >
        <h2 class="section__title">Qualification</h2>
        <span class="section__subtitle">My personal journey</span>

        <div
          class="qualification__container container grid services__container"
        >
          <div class="qualification__tabs">
            <div
              class="qualification__button button--flex qualification__active"
              data-target="#education"
            >
              <i class="uil uil-graduation-cap qualification__icon"></i>
              Education
            </div>
          </div>

          <div class="qualification__sections">
            <!--====== Qualification Content 1 ======-->
            <div
              class="qualification__content qualifiation__active services__content"
              data-content
              id="education"
            >
              <!--====== Qualification 1 ======-->
              <div class="qualification__data">
                <div>
                  <h3 class="qualification__title">SSLC</h3>
                  <span class="qualification__subtitle"
                    >S.V.S <br />High School</span
                  >
                  <div class="qualification__calender">
                    <i class="uil uil-calendar-alt"></i>
                    - 2019
                  </div>
                  <span
                    class="button button--flex button--small button--link services__button"
                  >
                    View More
                    <i class="uil uil-arrow-right button__icon"></i>
                  </span>
                  <div class="services__modal">
                    <div class="services__modal-content">
                      <h4 class="services__modal-title">
                        Class 10th Summary :
                      </h4>
                      <i class="uil uil-times services__modal-close"></i>
                      <ul class="services__modal-services grid">
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__moda-icon"
                          ></i>
                          <p>
                            Subjects studied: Science, Maths, English,
                            Social Studies,Kannada,Hindi.
                          </p>
                        </li>
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__moda-icon"
                          ></i>
                          <p>Scored 91%</p>
                        </li>
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__moda-icon"
                          ></i>
                          <p>Came runners up in inter-school Ball Badminton</p>
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>

                <div>
                  <span class="qualification__rounder"></span>
                  <span class="qualification__line"></span>
                </div>
              </div>

              <!--====== Qualification 2 ======-->
              <div class="qualification__data">
                <div></div>

                <div>
                  <span class="qualification__rounder"></span>
                  <span class="qualification__line"></span>
                </div>
                <div>
                  <h3 class="qualification__title">Class 12th</h3>
                  <span class="qualification__subtitle"
                    >Vidyodaya <br />Pre University College</span
                  >
                  <div class="qualification__calender">
                    <i class="uil uil-calendar-alt"></i>
                    - 2021
                  </div>
                  <span
                    class="button button--flex button--small button--link services__button"
                  >
                    View More
                    <i class="uil uil-arrow-right button__icon"></i>
                  </span>
                  <div class="services__modal">
                    <div class="services__modal-content">
                      <h4 class="services__modal-title">
                        Class 12th Summary :
                      </h4>
                      <i class="uil uil-times services__modal-close"></i>
                      <ul class="services__modal-services grid">
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__moda-icon"
                          ></i>
                          <p>
                            Subjects studied: Physics, Chemistry, Maths,
                            English, Statistics , Hindi.
                          </p>
                        </li>
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__moda-icon"
                          ></i>
                          <p>Scored 87.5%</p>
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>

              <!--====== Qualification 3 ======-->
              <div class="qualification__data">
                <div>
                  <h3 class="qualification__title">College</h3>
                  <span class="qualification__subtitle"
                    >Canara Enginnering College, Manglore</span
                  >
                  <div class="qualification__calender">
                    <i class="uil uil-calendar-alt"></i>
                    2021 - 2025
                  </div>
                  <span
                    class="button button--flex button--small button--link services__button"
                  >
                    View More
                    <i class="uil uil-arrow-right button__icon"></i>
                  </span>
                  <div class="services__modal">
                    <div class="services__modal-content">
                      <h4 class="services__modal-title">College Summary :</h4>
                      <i class="uil uil-times services__modal-close"></i>
                      <ul class="services__modal-services grid">
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__modal-icon"
                          ></i>
                          <p>
                            Studying core subjects of IT including DSA, Embedded
                            systems, Design analysis and algorithm, Operating
                            systems, and Computer architecture .
                          </p>
                        </li>
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__modal-icon"
                          ></i>
                          <p>Scored an aggregate of 8.50 CGPA till now.</p>
                        </li>
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__modal-icon"
                          ></i>
                          <p>
                            Student coordinator in media and
                            publication club of the college.
                          </p>
                        </li>
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__modal-icon"
                          ></i>
                          <p>
                            Club Advisor for GeekHub.
                          </p>
                        </li>
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__modal-icon"
                          ></i>
                          <p>
                            CodeBlaze hackathon winners under open innovation.
                          </p>
                        </li>
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__modal-icon"
                          ></i>
                          <p>
                            Runners in Edu-Vitality Hackathon in the track of AI in Education.
                          </p>
                        </li>
                        <li class="services__modal-service">
                          <i
                            class="uil uil-check-circle services__modal-icon"
                          ></i>
                          <p>
                            Finalist in Dark Pattern Buster Hackathon conducted by Department of Consumer Affairs of India.
                          </p>
                        </li>
                        
                      </ul>
                    </div>
                  </div>
                </div>

                <div>
                  <span class="qualification__rounder"></span>
                  <!--<span class="qualification__line"></span>-->
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!--=================== Portfolio ===================-->
      <section class="portfolio section" id="portfolio">
        <h2 class="section__title">Projects</h2>
        <span class="section__subtitle">Most recent work</span>

        <div class="portfolio__container container swiper-container">
          <div class="swiper-wrapper">
            <!-- ------------------------portfollio 1-------------------- -->
            <div class="portfolio__content grid swiper-slide">
              <img src="assets/img/portfolio5.png" class="portfolio__img" />

              <div class="portfolio__data">
                <h3 class="portfolio__title">
                  DarkSurfer-Extension
                </h3>
                <p class="portfolio__description">
                  DarkSurfer-Extension, is a project based on the application of advanced Language Models LMs to detect and eliminate dark patterns on websites. It aims to improve user-awareness, exposing real-time of devious design practices in situ. It helps make the internet more user-friendly by using its novel LMs and popular LM-based models, such as RoBERTa, BERT, and XLNet.
                </p>
                <a
                  href="https://github.com/Venkateeshh/DarkSurfer-Extension"
                  class="button button--flex button--small portfolio__button"
                >
                  GitHub Repository
                  <i class="uil uil-external-link-alt button__icon"></i>
                </a>
                <a
                  href="https://darksurfer.streamlit.app/"
                  class="button button--flex button--small portfolio__button"
                >
                  See Live
                  <i class="uil uil-external-link-alt button__icon"></i>
                </a>
              </div>
            </div>
            <!-- ------------------------portfollio 2-------------------- -->

            <div class="portfolio__content grid swiper-slide">
              <img src="assets/img/portfolio1.png" class="portfolio__img" />

              <div class="portfolio__data">
                <h3 class="portfolio__title">
                  Responsive-Weather-Forecast-Website
                </h3>
                <p class="portfolio__description">
                  This project is a weather website that provides live weather
                  updates and forecasts based on your location. Stay informed
                  about current weather conditions, temperature, and more.
                  Explore interactive maps, hourly/daily forecasts, and helpful
                  insights. Stay ahead of the forecast and make the most of your
                  day!
                </p>
                <a
                  href="https://github.com/Venkateeshh/Weather-App"
                  class="button button--flex button--small portfolio__button"
                >
                  GitHub Repository
                  <i class="uil uil-external-link-alt button__icon"></i>
                </a>
                <a
                  href="https://venkateeshh.github.io/Weather-App/"
                  class="button button--flex button--small portfolio__button"
                >
                  See Live
                  <i class="uil uil-external-link-alt button__icon"></i>
                </a>
              </div>
            </div>

            <!-- ------------------------portfollio 3-------------------- -->
            <div class="portfolio__content grid swiper-slide">
              <img src="assets/img/portfolio2.png" class="portfolio__img" />

              <div class="portfolio__data">
                <h3 class="portfolio__title">Spotify-Clone</h3>
                <p class="portfolio__description">
                  Spotify Clone is a web app developed using HTML, CSS, and
                  JavaScript. It recreates Spotify's interface and features,
                  allowing users to browse, search, and play songs, create
                  playlists, and discover new music. Responsive design ensures a
                  seamless experience on any device. Contributions are welcome!
                </p>
                <a
                  href="https://github.com/Venkateeshh/Spotify-Clone"
                  class="button button--flex button--small portfolio__button"
                >
                  GitHub Repository
                  <i class="uil uil-external-link-alt button__icon"></i>
                </a>
                <a
                  href="https://venkateeshh.github.io/Spotify-Clone/"
                  class="button button--flex button--small portfolio__button"
                >
                  See Live
                  <i class="uil uil-external-link-alt button__icon"></i>
                </a>
              </div>
            </div>
            <!-- ------------------------portfollio 4-------------------- -->
            <div class="portfolio__content grid swiper-slide">
              <img src="assets/img/portfolio3.png" class="portfolio__img" />

              <div class="portfolio__data">
                <h3 class="portfolio__title">Language Translator</h3>
                <p class="portfolio__description">
                  This language translator web app is a user-friendly tool built
                  with HTML, CSS, and JavaScript. It leverages Google Translate
                  API to seamlessly translate text between multiple languages.
                  The app features a simple interface, ensuring smooth
                  performance across devices..
                </p>
                <a
                  href="https://github.com/Venkateeshh/Js-Language-Translator"
                  class="button button--flex button--small portfolio__button"
                >
                  GitHub Repository
                  <i class="uil uil-external-link-alt button__icon"></i>
                </a>
                <a
                  href="https://venkateeshh.github.io/Js-Language-Translator/"
                  class="button button--flex button--small portfolio__button"
                >
                  See Live
                  <i class="uil uil-external-link-alt button__icon"></i>
                </a>
              </div>
            </div>

            <!-- ------------------------portfollio 5-------------------- -->
            <div class="portfolio__content grid swiper-slide">
              <img src="assets/img/portfolio4.png" class="portfolio__img" />

              <div class="portfolio__data">
                <h3 class="portfolio__title">Sorting Visualizer</h3>
                <p class="portfolio__description">
                  Sorting Visualizer is a Java-based project that allows users
                  to visualize various sorting algorithms in action using a
                  Graphical User Interface (GUI). It provides an interactive and
                  educational way to understand how different sorting algorithms
                  work by visually demonstrating their step-by-step sorting
                  process.
                </p>
                <a
                  href="https://github.com/Venkateeshh/Sorting-Visualizer"
                  class="button button--flex button--small portfolio__button"
                >
                  GitHub Repository
                  <i class="uil uil-external-link-alt button__icon"></i>
                </a>
                <a
                  href="https://www.linkedin.com/posts/venkatesh-kamath-_algorithmdesign-sortingvisualizer-javaprojects-activity-7095437035125043200-fWDl?utm_source=share&utm_medium=member_desktop"
                  class="button button--flex button--small portfolio__button"
                >
                  See Live
                  <i class="uil uil-external-link-alt button__icon"></i>
                </a>
              </div>
            </div>
          </div>

          <!-- add arrows -->
          <div class="swiper-button-next">
            <i class="uil uil-angle-right-b swiper-portfolio-icon"></i>
          </div>
          <div class="swiper-button-prev">
            <i class="uil uil-angle-left-b swiper-portfolio-icon"></i>
          </div>
          <!-- add pagination -->
          <div class="swiper-pagination"></div>
        </div>
      </section>

      <!--===================== Contact Me =====================-->
      <section class="contact section" id="contact">
        <h2 class="section__title">Contact Me</h2>
        <span class="section__subtitle">Get in touch</span>

        <div class="contact__container container grid">
          <div>
            <div class="contact__information">
              <i class="uil uil-calling contact__icon"></i>

              <div>
                <h3 class="contact__title">Contact Me</h3>
                <span class="contact__subtitle"
                  ><a href="tel:6362243314"></a>6362243314</span
                >
              </div>
            </div>

            <div class="contact__information">
              <i class="uil uil-envelope-minus contact__icon"></i>

              <div>
                <h3 class="contact__title">Email</h3>
                <span class="contact__subtitle"
                  >rkamathvenkatesh@gmail.com</span
                >
              </div>
            </div>

            <div class="contact__information">
              <i class="uil uil-map-marker contact__icon"></i>

              <div>
                <h3 class="contact__title">Location</h3>
                <span class="contact__subtitle"
                  >Manglore, Karnataka, India</span
                >
              </div>
            </div>
          </div>

          <form action="" class="contact__form grid">
            <div class="contact__inputs grid">
              <div class="contact__content">
                <label for="" class="content__label">Name</label>
                <input type="text" class="contact__input" />
              </div>

              <div class="contact__content">
                <label for="" class="content__label">Email</label>
                <input type="Email" class="contact__input" />
              </div>
            </div>

            <div class="contact__content">
              <label for="" class="content__label">Message</label>
              <textarea
                name=""
                id=""
                cols="0"
                rows="7"
                class="contact__input"
              ></textarea>
            </div>

            <div>
              <a
                href=" mailto: rkamathvenkatesh@gmail.com?subject=Testing out mailto! &body=This is only a test!"
                class="button button--flex"
              >
                Send Message
                <i class="uil uil-message button__icon"></i>
              </a>
            </div>
          </form>
        </div>
      </section>
    </main>

    <!--================== Footer ===============-->
    <footer class="footer">
      <div class="footer__bg">
        <div class="footer__container container grid">
          <div>
            <h1 class="footer__title">Venkatesh</h1>
            <span class="footer__subtitle"
              >Information Science Engineering Student</span
            >
          </div>

          <ul class="footer__links">
            <li>
              <a href="#qualification" class="footer__link">Qualification</a>
            </li>
            <li>
              <a href="#portfolio" class="footer__link">Portfolio</a>
            </li>
            <li>
              <a href="#contact" class="footer__link">Contact-Me</a>
            </li>
          </ul>

          <div class="footer__socials">
            <a
              href="https://www.instagram.com/venkateeshh/"
              class="footer__social"
              target="__blank"
            >
            <i class="fa-brands fa-instagram"></i>
            </a>

            <a
              href="https://twitter.com/Venkateeshhh"
              target="__blank"
              class="footer__social"
            >
            <i class="fa-brands fa-x-twitter"></i>
            </a>
          </div>
        </div>

        <p class="footer__copy">&#169; Venkatesh. All right reserved</p>
      </div>
    </footer>

    <!--================== SCROLL TOP ==================-->
    <a href="#" class="scrollup" id="scroll-up">
      <i class="uil uil-arrow-up scrollup__icon"></i>
    </a>

    <script type="text/javascript" src="assets/swiper-bundle.min.js"></script>
    <script src="https://kit.fontawesome.com/2205d59d52.js" crossorigin="anonymous"></script>
    <script src="assets/ptj.js"></script>
  </body>
</html>
