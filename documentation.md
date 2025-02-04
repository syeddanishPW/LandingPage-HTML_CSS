 **Documentation for Your Web Project (Including Animations & Keyframes)**  
This documentation provides an overview of **StudySync** web project, explaining its **HTML, CSS, animations, and responsiveness** in a beginner-friendly manner.

---

**1. Overview**  
The **StudySync** project is a **responsive, modern landing page** designed for an online learning platform. It includes:  
✔ **Navigation bar** with internal links  
✔ **Hero section** with call-to-action buttons  
✔ **Feature highlights** with animations  
✔ **Testimonials section** with sliding effects  
✔ **Newsletter signup**  
✔ **Animated elements using CSS keyframes**  

The project is built using:  
- **HTML** for structure  
- **CSS** for styling, responsiveness, and animations  
- **Google Fonts & CSS Variables** for design consistency  

---

**2. File Structure**
```
/StudySync
│── index.html    # Main HTML file
│── style.css     # CSS file for styling & animations
│── assets/       # Folder for images & icons
```

---

**3. HTML Explanation (`index.html`)**
The **HTML file** provides the structure of the web page.  

**(a) Navigation Bar**
```html
<header class="header-content">
    <a href="#logo" class="logo">
        <img src="/assets/StudySyn.svg" alt="logo" class="logo-icon">
        <span class="logo-text">StudySync</span>
    </a>
    <nav class="nav">
        <a href="#home" class="nav-link">Home</a>
        <a href="#features" class="nav-link">Features</a>
        <a href="#pricing" class="nav-link">Pricing</a>
        <a href="#blog" class="nav-link">Blog</a>
        <a href="#about" class="nav-link">About</a>
    </nav>
    <a href="#contact" class="contact-btn">Contact Us</a>
</header>
```
- **Logo & Branding**
- **Navigation Menu**
- **CTA Button (Contact Us)**  

---

**(b) Hero Section (Includes Animations)**
```html
<section class="main-sect">
    <div class="content-left">
        <p class="section-label">Very proud to introduce</p>
        <h1 class="section-title animate-text">Seamless Learning for Brighter Futures</h1>
        <p class="section-desc">Our innovative platform offers an effortless approach to learning...</p>
        <div class="button-grp">
            <a href="#start" class="start-btn">Start Now</a>
            <a href="#tour" class="tour-btn">Take Tour</a>
        </div>
    </div>
</section>
```
- **Animated Text (`animate-text`)** applied using CSS keyframes.  
- **Buttons with Hover Effects**  

---

**(c) Features Section (With Animations)**
```html
<div class="feature-grid">
    <div class="feature-card fade-in">
        <div class="icon-container">
            <img src="/assets/PersonalizedLearn.svg" class="feature-svg">
        </div>
        <div class="feature-info">
            <div class="feature-title">Personalized Learning</div>
            <div class="feature-desc">AI-based learning experience tailored to student needs.</div>
        </div>
    </div>
</div>
```
- **Class `fade-in` adds animation when the section appears on the screen.**  
- **Feature cards are animated for better UI experience.**  

---

**4. CSS Explanation (`style.css`)**
 **(a) Global Styling**
```css
:root {
    --primary-color: #6366f1;
    --text-color: #333;
    --background-color: #ffffff;
}
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Inter", sans-serif;
}
```
- Uses **CSS Variables** for easy theme management.  
- Ensures consistent styling across the webpage.  

---

**(b) Navigation Styling**
```css
.nav-link {
    color: #718096;
    font-size: 1.125rem;
    font-weight: 600;
    transition: color .2s;
}
.nav-link:hover {
    color: var(--primary-color);
}
```
- **Hover effect** on navigation links.  

---

**(c) Animations & Keyframes**
**1 Fade-In Animation for Main Section**  
```css
.content-left{
    text-align: center;
    animation: slideFromLeft 1s ease forwards;
    opacity: 0;
}

@keyframes slideFromLeft{
    0%{
        opacity: 0;
        transform: translateX(-100%);
    }

    100%{
        opacity: 1;
        transform: translateX(0);
    }   
}
```
- **Main section fade in when they appear.**  

---

 **(d) Responsive Design- Mobile First Approach**
```css
@media screen and (min-width: 768px) {
    .nav {
        display: flex;
    }
}

@media screen and (max-width: 768px){
    .menu-btn{
        display: block;
    }   
}
```
- **Hides navigation menu on small screens**.  
- **Uses a mobile-friendly layout.**  

---

**5. Key Features**
✔ **Modern & Responsive** – Works on all screen sizes.  
✔ **Smooth Animations** – CSS keyframes for text and section reveals.  
✔ **Optimized Navigation** – Clean, structured header for easy access.  
✔ **SEO Friendly** – Uses semantic HTML (`<header>`, `<section>`, `<footer>`).  

---

**6. How to Run the Project**
1. **Download the files** (`index.html` & `style.css`).  
2. Keep both files in the **same folder**.  
3. Open `index.html` in a browser (Chrome, Firefox, Edge).  
4. The animations and responsive design will be visible.  

---

**Conclusion**
This documentation explains how the **StudySync** web project is structured, styled, and animated. The use of **CSS keyframes** ensures smooth transitions, improving user experience.