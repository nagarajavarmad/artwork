# Artwork

The project provides landing page for a service which provides custom designs based on user requirements

The project website is deployed via github pages and can be accessed from https://nagarajavarmad.github.io/artwork/

The project is developed as a pure html based static website.

## Technologies used

- HTML
- CSS
- Javascript

## Libraries used

- Bootstrap CSS https://getbootstrap.com/
- Fontawesome icons https://fontawesome.com/
- Swiper js for testimonial carousel https://swiperjs.com/
- Google Maps embed

## Website Description

The website has the following pages

Landing page or index page which contains information about the artwork service and links to

- Categories page which lists the available categories of designs that the service provides. From the category page, user can click on individual category to see listing of the current category.
- Individual category page shows a list of designs that with an image,title and description
- Login page from which user can login/register
- Contact page to which show the contact details of the business

NOTE:

Currently only single category page is implemented. By it should be trivial to expand the implementation to have different category pages for different categories.

## Technical Implementation

The pages use extensively bootstrap Grid css for its flexbox layout requirements

Login/Register forms use bootstrap form controls

Custom css is used throught out the pages where boostrap provided css cannot be used to acheive desired effect.

### CSS Structure

All the global css classes that are required across diffierent pages are added to `main.css` file. This file will be loaded for all pages

Each individual page's specific css classes are stored in their respective css files with the same name and they are only laoded on their corresponding html pages

### Responsive Design

Bootstrap CSS Grid provides responsive classes to adapt the implementation for different devices.

Example usecase from the project:

In `index.html` page, we have a hero section with service description and an image on the right. Boostrap responsiveness is mobile first. So, I implemented the requirement as two columns in a row that take full width on mobile and eqaul width on desktop. On mobile, when the columns take full width, they will wrap into new line. So I am using `flex-wrap-reverse` class to reverse the columns in this case. This gives the desired effect of

On Mobile

- Image column is shown first
- Text column is shown below it

On Desktop

- Text column is on the left
- Image column is on the right

## References

1. Project layout, text, image inspiration https://www.designcrowd.com/
2. Icons from https://fontawesome.com/
3. Images from https://dribbble.com/
