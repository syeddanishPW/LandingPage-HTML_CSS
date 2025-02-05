 **Documentation for Your Web Project (Including Animations & Keyframes)**  
This documentation provides an overview of **StudySync** web project, explaining its **HTML, CSS, animations, and responsiveness** in a beginner-friendly manner.

---

**1. Overview**  
The **StudySync** project is a **responsive, modern landing page** designed for an online learning platform. It includes:  
✔ **Navigation bar** with internal links  
✔ **Hero section** with call-to-action buttons  
✔ **Testimonials section** with sliding effects  
✔ **Newsletter signup section**  
✔ **Animated elements using CSS keyframes**  

The project is built using:  
- **HTML** for structure  
- **CSS** for styling, responsiveness, and animations  
- **Google Fonts & CSS Variables** for design consistency  

---

**1. File Structure**
```
/StudySync
│── index.html    # Main HTML file
│── style.css     # CSS file for styling & animations
│── assets/       # Folder for images & icons
```

---

**2. HTML Explanation (`index.html`)**
The **HTML file** provides the structure of the web page.  

**(a) Hero Section (Includes Animations)**
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
- **Buttons with Hover Effects**
  
**(b) Testimonial Section**
```html
<div class="testimonial-container">
      <div class="testimonial-content">
        <h2 class="testimonial-title">What Others Say About Us</h2>
        <div class="test-grid">
          <!-- card 1 -->
          <div class="testimonial-card">
            <div class="testimonial-text">
              “StudySync revolutionized my classroom! Engaging content and
              teacher resources make learning enjoyable. Highly recommended for
              educators.”
            </div>
            <div class="testimonial-avatar">
              <img src="/assets/avatar1.png" alt="" />
            </div>
            <div class="testimonial-details">
              <h3>Sarah Johnson</h3>
              <p>8th Grade English Teacher</p>
            </div>
          </div>
```
- **Used CSS Grid and Flex**
- **CSS Transform Property**
- **Hover Effects**

---

**3. CSS Explanation (`style.css`)**
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
---

**(b) Animations & Keyframes**
**1 Fade-In Animation for Main Section**  
```css
.content-left{
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
1. **Download the files and assets** (`index.html` & `style.css`).  
2. Keep both files in the **same folder**.  
3. Open `index.html` in a browser (Chrome, Firefox, Edge).  
4. The animations and responsive design will be visible.  

---

**Conclusion**
This documentation explains how the **StudySync** web project is structured, styled, and animated. The use of **CSS keyframes** ensures smooth transitions, improving user experience.  
