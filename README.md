1. Overview

The University Annual Carnival project is a responsive and interactive webpage designed to provide event details, registration, schedule, and media gallery for the university carnival. The project includes:

✔ Event registration form for participants
✔ Schedule table displaying event timings and locations
✔ Media gallery with embedded YouTube videos
✔ File upload section for user contributions (photos & clips)
✔ Responsive design ensuring accessibility on all devices

Technologies Used:
HTML for webpage structure
CSS for styling and animations
Google Fonts for enhanced typography

2. File Structure

/UniversityCarnival
│── index.html      # Main HTML file
│── style.css       # CSS file for styling & animations

3. HTML Explanation (index.html)

✔ Explanation:
```html
<fieldset>``` groups related form elements, improving structure and accessibility.
```html
<legend>``` provides a title for better readability.
✔ Issue: YouTube doesn’t allow direct embedding via ```<video>``` and <source>.
Instead, use an <iframe> like this:
```html
 <div class="media-gallery">
      <iframe src="https://www.youtube.com/embed/8htJwPTFvRo" frameborder="0" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/iS-lWnlZuQ8" frameborder="0" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/nXbXNB9E71o" frameborder="0" allowfullscreen></iframe>
    </div>
```

Form Fields: Users enter their name, email, contact number, and department.
Dropdown Menu: Allows users to select their department.
Button: Submits the registration form.
Ensures video embeds are responsive on smaller screens.

5. Key Features

✔ Smooth Animations: CSS keyframes for transitions.
✔ User-Friendly Forms: Easy registration process.
✔ Interactive Media Gallery: Embedded videos for engagement.

6. How to Run the Project

Download the files (index.html & style.css).

Place both files in the same directory.

Open index.html in a browser.

Experience the animations and responsive design.

7. Future Improvements
Adding CSS for better styling and user experience.
Implementing JavaScript validation to enhance form validation before submission.
Integrating a backend (e.g., PHP, Node.js) to process and store submitted applications.

Conclusion

This documentation outlines the structure, styling, and animations of the University Annual Carnival web project. The use of CSS animations, transitions, and a responsive layout ensures an engaging and accessible user experience.
