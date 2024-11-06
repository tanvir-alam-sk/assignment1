A simple, responsive image carousel built using only HTML and CSS. This project demonstrates how to create a basic image slider without JavaScript by leveraging CSS animations and radio buttons.

Demo
The carousel displays two images per slide and can be navigated using dots below the slider.


Features
Responsive: Adjusts to different screen sizes.
Pure CSS: No JavaScript required.
Easy Customization: You can easily add more slides or customize the appearance.
How It Works
The carousel relies on hidden radio buttons and CSS :checked selectors to create a sliding effect between the images.

Radio Buttons: Each slide is associated with a hidden radio button. When a radio button is selected, CSS selectors target the corresponding slide.
Flexbox Layout: Used to position the images within each slide and create the side-by-side effect.
CSS Transforms: The active slide is shown by shifting the .carousel__slides container with transform: translateX(...).
Getting Started
Prerequisites
A modern web browser to view the project.
Installation
Clone the repository:

bash
Copy code
git clone [https://github.com/your-username/css-only-carousel.git](https://github.com/tanvir-alam-sk/assignment1)
Navigate to the project folder:

bash
Copy code
cd css-only-carousel
Open the index.html file in your browser to view the carousel.

Customization
Add More Slides: To add more slides, include additional <div class="carousel__slide"> elements in the .carousel__slides container and update the CSS transform rules to match.
Change Image Size: Adjust the .carousel__slide img width or the container dimensions to resize the images.
Code Overview
html
Copy code
<div class="carousel">
  <input type="radio" name="carousel" id="slide1" checked>
  <input type="radio" name="carousel" id="slide2">
  <input type="radio" name="carousel" id="slide3">

  <div class="carousel__slides">
    <div class="carousel__slide">
      <img src="https://via.placeholder.com/300x300?text=Image+1" alt="Image 1">
      <img src="https://via.placeholder.com/300x300?text=Image+2" alt="Image 2">
    </div>
    <div class="carousel__slide">
      <img src="https://via.placeholder.com/300x300?text=Image+3" alt="Image 3">
      <img src="https://via.placeholder.com/300x300?text=Image+4" alt="Image 4">
    </div>
    <!-- Additional slides go here -->
  </div>

  <div class="carousel__nav">
    <label for="slide1"></label>
    <label for="slide2"></label>
    <label for="slide3"></label>
  </div>
</div>
