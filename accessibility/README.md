# Accessibility

## Resources
**Read or watch:**
- [Accessibility is not a feature. — Ethan Marcotte](https://ethanmarcotte.com/wrote/accessibility-is-not-a-feature/)
- [How to Meet WCAG (Quickref Reference](https://www.w3.org/WAI/WCAG21/quickref/?versions=2.0)
- [Web Accessibility Guidebook for Developers](https://www.telerik.com/blogs/web-accessibility-guidebook-for-developers?fbclid=IwAR3v8sqaMyuAYfa14dZJpDKqJd-v8qKfaKeEvZJRKTcRIOabNnYGPo4rA7U)
- [Testing with assistive technologies - Service Manual - GOV.UK](https://www.gov.uk/service-manual/technology/testing-with-assistive-technologies)
- [A11Y Style Guide](https://a11y-style-guide.com/style-guide/)
- [Building Pylon-Free Web Pages: An Intro to Web Accessibility](https://engineering.vena.io/building-pylon-free-web-pages-an-intro-to-web-accessibility/)
- [I Threw Away my Mouse - 24 Accessibility](https://www.24a11y.com/2018/i-threw-away-my-mouse/)
- [I Used a Switch Control for a Day - 24 Accessibility](https://www.24a11y.com/2018/i-used-a-switch-control-for-a-day/)
- [The Myths of Color Contrast Accessibility](https://uxmovement.com/buttons/the-myths-of-color-contrast-accessibility/)
- [IAAP Certification](https://www.accessibilityassociation.org/s/certification)
- [Accessibility Blog | Deque Systems](https://www.deque.com/blog/)
- [Tink - Léonie Watson – On technology, food & life in the digital age](https://tink.uk/)
- [Articles » Simply Accessible](https://www.levelaccess.comarticles/)
- [Accessibility Weekly](https://a11yweekly.com/)
- [European label (Web Accessibility): Euracert - Home page](http://www.euracert.org/en/)
- [Section508.gov | GSA Government-wide IT Accessibility Program](https://www.section508.gov/)
- [images archive]()

## Learning Objectives
- ARIA’s main purpose
- WCAG conformance levels (A, AA and AAA)
- The importance of Web Accessibility
- Tools to use for Web Accessibility

## Requirements
- Allowed editors: **vi**, **vim**, **emacs**
- HTML and CSS have been rendered on Chrome 78 or more.



Curriculum
Short Specializations Average: 110.2%
Accessibility
HTMLCSSFront-end

    By: David Dias, Senior Software Engineer at HomeX
    Weight: 1
    Ongoing second chance project - started Oct 30, 2023 6:00 AM, must end by Nov 13, 2023 6:00 AM
    An auto review will be launched at the deadline

In a nutshell…

    Auto QA review: 0.0/0 mandatory & 0.0/104 optional
    Altogether:  0.0%
        Mandatory: no mandatory tasks
        Optional: 0.0%

Concepts

For this project, we expect you to look at this concept:

    A Crash Course on Accessibility

Resources

Read or watch:

    Accessibility is not a feature. — Ethan Marcotte
    How to Meet WCAG (Quickref Reference
    Web Accessibility Guidebook for Developers
    Testing with assistive technologies - Service Manual - GOV.UK
    A11Y Style Guide
    Building Pylon-Free Web Pages: An Intro to Web Accessibility
    I Threw Away my Mouse - 24 Accessibility
    I Used a Switch Control for a Day - 24 Accessibility
    The Myths of Color Contrast Accessibility
    IAAP Certification
    Accessibility Blog | Deque Systems
    Tink - Léonie Watson – On technology, food & life in the digital age
    Articles » Simply Accessible
    Accessibility Weekly
    European label (Web Accessibility): Euracert - Home page
    Section508.gov | GSA Government-wide IT Accessibility Program

Learning Objectives

At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

    ARIA’s main purpose
    WCAG conformance levels (A, AA and AAA)
    The importance of Web Accessibility
    Tools to use for Web Accessibility

Requirements

    Allowed editors: vi, vim, emacs
    A README.md at the root of the project directory is mandatory
    HTML and CSS have been rendered on Chrome 78 or more.

Quiz questions
Great! You've completed the quiz successfully! Keep going! (Show quiz)
Tasks
0. make the "works" card focus visible
#advanced
Score: 0.0% (Checks completed: 0.0%)

Start with this 00-styles.css file:
Click to expand/hide file contents

You can use it with this 00-index.html file:

<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
    <title>Homepage - Techium</title>
    <meta name="description" content="Description of the page less than 150 characters">
    <link rel="icon" type="image/x-icon" href="../images/favicon.ico">
    <link rel="icon" type="image/png" href="../images/favicon.png">
    <link href="https://fonts.googleapis.com/css?family=Open+Sans:400,700|Raleway:700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="00-styles.css">
  </head>
  <body>
    <!– Header –>
    <header class="header" data-section-theme="dark">
      <div class="container">
        <div class="header-container">
          <div class="header-logo">
            <a href="/">
              <img src="../images/logo-white.png" alt="Techium logo" width="160" height="40">
            </a>
          </div>
          <input class="menu-btn" type="checkbox" id="menu-btn" />
          <label class="menu-icon" for="menu-btn">
            <span class="navicon"></span>
          </label>
          <nav class="navbar-menu">
            <ul class="nav">
              <li class="nav-item">
                <a href="/" class="nav-link">Home</a>
              </li>
              <li class="nav-item">
                <a href="#services" class="nav-link">Services</a>
              </li>
              <li class="nav-item">
                <a href="#works" class="nav-link">Works</a>
              </li>
              <li class="nav-item">
                <a href="#about" class="nav-link">About</a>
              </li>
              <li class="nav-item">
                <a href="#latest_news" class="nav-link">Latest news</a>
              </li>
              <li class="nav-item">
                <a href="#testimonials" class="nav-link">Testimonials</a>
              </li>
              <li class="nav-item">
                <a href="#contact" class="nav-link">Contact</a>
              </li>
              <li class="nav-item">
                <form action="#" method="post" class="form-search">
                  <input type="search" name="q" id="search-input" placeholder="Search..." aria-label="Search through site content">
                  <button class="search-button">
                    <svg viewbox="0 0 512 512" xmlns="http://www.w3.org/2000/svg" width="20" height="20" class="search-icon">
                      <title>
                        Search icon
                      </title>
                      <path d="M508.5 468.9L387.1 347.5c-2.3-2.3-5.3-3.5-8.5-3.5h-13.2c31.5-36.5 50.6-84 50.6-136C416 93.1 322.9 0 208 0S0 93.1 0 208s93.1 208 208 208c52 0 99.5-19.1 136-50.6v13.2c0 3.2 1.3 6.2 3.5 8.5l121.4 121.4c4.7 4.7 12.3 4.7 17 0l22.6-22.6c4.7-4.7 4.7-12.3 0-17zM208 368c-88.4 0-160-71.6-160-160S119.6 48 208 48s160 71.6 160 160-71.6 160-160 160z"/>
                    </svg>
                  </button>
                </form>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </header>
    <!– Main –>
    <main>
      <h1 class="visually-hidden">Homepage</h1>
      <!– Hero section –>
      <section class="section-hero hero-homepage" data-section-theme="dark">
        <div class="container">
          <div class="section-body">
            <section class="section-inner">
              <h2 class="section-title">We help you building your brand!</h2>
              <a href="#" class="button">Get Started</a>
            </section>
          </div>
        </div>
      </section>
      <!– Services section –>
      <section id="services" class="section section-services">
        <div class="container">
          <header class="section-header">
            <h2 class="section-title">Services</h2>
            <p class="section-tagline">We work with you</p>
          </header>
          <div class="section-body">
            <ul class="row">
              <li class="col-1-3">
                <div class="card-services">
                  <h3 class="card-title"><a href="#">Design & Concept</a></h3>
                </div>
              </li>
              <li class="col-1-3">
                <div class="card-services">
                  <h3 class="card-title"><a href="#">Digital Strategy</a></h3>
                </div>
              </li>
              <li class="col-1-3">
                <div class="card-services">
                  <h3 class="card-title"><a href="#">Content Strategy</a></h3>
                </div>
              </li>
              <li class="col-1-3">
                <div class="card-services">
                  <h3 class="card-title"><a href="#">UX Design</a></h3>
                </div>
              </li>
              <li class="col-1-3">
                <div class="card-services">
                  <h3 class="card-title"><a href="#">Web Development</a></h3>
                </div>
              </li>
              <li class="col-1-3">
                <div class="card-services">
                  <h3 class="card-title"><a href="#">Social Media</a></h3>
                </div>
              </li>
            </ul>
          </div>
        </div>
      </section>
      <!– Works section –>
      <section id="works" class="section section-works" data-section-theme="dark">
        <div class="container">
          <header class="section-header">
            <h2 class="section-title">Works</h2>
            <p class="section-tagline">Take a look in our portfolio</p>
          </header>
          <div class="section-body">
            <ul class="row">
              <li class="col-1-3">
                <article class="card-work">
                  <div class="card-outer">
                    <div class="card-image">
                      <img src="../images/pic-work-01.jpg" alt="">
                    </div>
                    <div class="card-inner">
                      <h3 class="card-title"><a href="#">Interior Design</a></h3>
                    </div>
                  </div>
                </article>
              </li>
              <li class="col-1-3">
                <article class="card-work">
                  <div class="card-outer">
                    <div class="card-image">
                      <img src="../images/pic-work-02.jpg" alt="">
                    </div>
                    <div class="card-inner">
                      <h3 class="card-title"><a href="#">Web Development</a></h3>
                    </div>
                  </div>
                </article>
              </li>
              <li class="col-1-3">
                <article class="card-work">
                  <div class="card-outer">
                    <div class="card-image">
                      <img src="../images/pic-work-03.jpg" alt="">
                    </div>
                    <div class="card-inner">
                      <h3 class="card-title"><a href="#">Personal Development</a></h3>
                    </div>
                  </div>
                </article>
              </li>
            </ul>
          </div>
        </div>
      </section>
      <!– About Us section –>
      <section id="about" class="section section-about-us">
        <div class="container">
          <header class="section-header">
            <h2 class="section-title">About us</h2>
            <p class="section-tagline">Everything about us</p>
          </header>
          <div class="section-body">
            <div class="row">
              <div class="col-1-2">
                <img
                  sizes="(max-width: 3000px) 40vw, 1200px"
                  srcset="
                  ../images/responsive/about-us_icoxoo_c_scale,w_380.jpg 380w,
                  ../images/responsive/about-us_icoxoo_c_scale,w_853.jpg 853w,
                  ../images/responsive/about-us_icoxoo_c_scale,w_1200.jpg 1200w"
                  src="../images/responsive/about-us_icoxoo_c_scale,w_1200.jpg"
                  alt="">
              </div>
              <div class="col-1-2">
                <h3>Who are we</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum, omnis expedita! Eum, praesentium cumque accusantium rem, sit quaerat est nisi ratione, deserunt ducimus quidem iste dicta quibusdam atque maxime cum!</p>
                <h3>Our culture</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum, omnis expedita! Eum, praesentium cumque accusantium rem, sit quaerat est nisi ratione, deserunt ducimus quidem iste dicta quibusdam atque maxime cum!</p>
                <h3>How we work</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum, omnis expedita! Eum, praesentium cumque accusantium rem, sit quaerat est nisi ratione, deserunt ducimus quidem iste dicta quibusdam atque maxime cum!</p>
              </div>
            </div>
          </div>
          <div class="section-footer">
            <a href="about-us.html" class="button">Learn more about us</a>
          </div>
        </div>
      </section>
      <!– Latest news section –>
      <section id="latest_news" class="section section-latest-news">
        <div class="container">
          <header class="section-header">
            <h2 class="section-title">Latest News</h2>
          </header>
          <div class="section-body">
            <ul class="row">
              <li class="col-1-3">
                <article class="card-blog">
                  <div>
                    <img
                    sizes="(max-width: 2250px) 40vw, 900px"
                    srcset="
                      ../images/responsive/pic-article-01_l2waac_c_scale,w_380.jpg 380w,
                      ../images/responsive/pic-article-01_l2waac_c_scale,w_673.jpg 673w,
                      ../images/responsive/pic-article-01_l2waac_c_scale,w_900.jpg 900w"
                      src="../images/responsive/pic-article-01_l2waac_c_scale,w_900.jpg"
                    alt="">
                  </div>
                  <p class="card-category">Career</p>
                  <h3><a href="#">Hoc loco tenere se Triarius non potuit.</a></h3>
                  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id Sextilius factum negabat. Quo tandem modo? At eum nihili facit; Quae contraria sunt his, malane?</p>
                  <small>By Kelly D.</small>
                </article>
              </li>
              <li class="col-1-3">
                <article class="card-blog">
                  <div>
                    <img
                    sizes="(max-width: 2250px) 40vw, 900px"
                    srcset="
                      ../images/responsive/pic-article-02_xe0wgi_c_scale,w_380.jpg 380w,
                      ../images/responsive/pic-article-02_xe0wgi_c_scale,w_682.jpg 682w,
                      ../images/responsive/pic-article-02_xe0wgi_c_scale,w_900.jpg 900w"
                      src="../images/responsive/pic-article-02_xe0wgi_c_scale,w_900.jpg"
                    alt="">
                  </div>
                  <p class="card-category">Digital Life</p>
                  <h3><a href="#">Ut alios omittam, hunc appello, quem ille unum secutus est.</a></h3>
                  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Tum mihi Piso: Quid ergo? Tum ille: Ain tandem? Non autem hoc: igitur ne illud quidem. Sed quod proximum fuit non vidit. Nos commodius agimus. An nisi populari fama?</p>
                  <small>By William A.</small>
                </article>
              </li>
              <li class="col-1-3">
                <article class="card-blog">
                  <div>
                    <img
                    sizes="(max-width: 2250px) 40vw, 900px"
                    srcset="
                      ../images/responsive/pic-article-03_hzlhrf_c_scale,w_380.jpg 380w,
                      ../images/responsive/pic-article-03_hzlhrf_c_scale,w_679.jpg 679w,
                      ../images/responsive/pic-article-03_hzlhrf_c_scale,w_900.jpg 900w"
                    src="../images/responsive/pic-article-03_hzlhrf_c_scale,w_900.jpg"
                    alt="">
                  </div>
                  <p class="card-category">Social</p>
                  <h3><a href="#">Bestiarum vero nullum iudicium puto.</a></h3>
                  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Non igitur bene. Quid enim est a Chrysippo praetermissum in Stoicis? Pugnant Stoici cum Peripateticis. Prioris generis est docilitas, memoria; Apparet statim, quae sint officia, quae actiones.</p>
                  <small>By Frances J.</small>
                </article>
              </li>
            </ul>
          </div>
        </div>
      </section>
      <!– Testimonials section –>
      <section id="testimonial" class="section section-testimonial">
        <div class="container">
          <header class="section-header">
            <h2 class="section-title">Testimonials</h2>
            <p class="section-tagline">We are more than a digital company</p>
          </header>
          <div class="section-body">
            <ul class="row">
              <li class="col-1-3">
                <article class="card-testimonial">
                  <img src="../images/pic-person-01.jpg" alt="Yuri Y. avatar" width="100" height="100" class="card-avatar">
                  <blockquote class="card-quote">
                    <p>I am completely blown away. Thanks to Techium, we’ve just launched our 5th website!
                      <cite>Yuri Y.</cite>
                    </p>
                  </blockquote>
                </article>
              </li>
              <li class="col-1-3">
                <article class="card-testimonial">
                  <img src="../images/pic-person-02.jpg" alt="Dorrie S. avatar" width="100" height="100" class="card-avatar">
                  <blockquote class="card-quote">
                    <p>Thank you so much for your help. Techium company is awesome!
                      <cite>Dorrie S.</cite>
                    </p>
                  </blockquote>
                </article>
              </li>
              <li class="col-1-3">

