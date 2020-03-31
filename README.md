# Vigilant Security Systems Ltd

A live demo can be found here: https://grimsas.github.io/MS1/

![](readme\main.png)

Do you need brand-new security alarms to protect your Caterham, Banstead, Oxted or Warlingham property? Our experienced security company carries out installations and security alarm maintenance for domestic and commercial clients throughout the UK. Our fully-qualified technicians are available on an emergency basis for jobs at small to large-scale properties – from apartments and estates, to offices and industrial warehouses. We also provide free advice about a range of security alarms, plus obligation-free consultations.

## UX
The purpose of this project is to create static website for a installer of security systems, as the existing website http://www.vigilantsecurity.co.uk/ is visualy unpleasing, unresponsive and did not atract potential customers attention.

My goal was to make website as simple as possible, with responsive page layout, providing brief services overview, deals, contact form and other means of comunication and a physical address to visit.

## Features

Website use Bootstrap 4 and due to design and responsivenes had to add custom @media queries sizes as some responsive features didn't scale. All external links opens on the new tab. Some text use calc() funcion to scale to screen size and prevent unwanted wrap or overflow.

### Navbar

Navbar responsiveness achieved with Bootstrap. At first I've tried to use skewed menu items, but due to visual inconsistency left them at 0 degrees. Menu items use borders on one side on the large screens, and on the bottom on the small to medium screens, this achieved through @media queries and adding borders to the :nth-childs. Large screens have shadow on menu item hover, and smaller screens goes transperent. Also navbar gives visual scroll 'location' with a help of 'scrollspy'.

### Home

Basic cards with a brief company and services provided desctiption. Quick links to redirect to Home and Business content. Background image is overlayed with pattern image.

### Deals

Deal section has two images, as it doesn't scale, I've used  hide and show on certain breakpoints, so it will be consistent with the device size. Also text position, size and layout is diferent on various screens sizes.

### Services

For services I've used 'tiles' design and on every breakpoint it changes the layout, i.e. xlarge is 4 in the row, large is 3,  medium is 2 and small 1 tile. Created a 'dummy' tile, whitch is visible on the large screen only to preserve layout consistency.

### Contact Us

Contact us has a enquiry form, Map, Adress, phone and email, and dummy copyright information. 

## Technologies Used

1.HTML
2.CSS
3.Bootstrap 4

## Testing

Is it Mobile Friendly? Yes, according to google test tool: https://search.google.com/test/mobile-friendly?id=VSx_HbNf0Y7hpI-Ax97P3w

Both https://validator.w3.org/ and https://jigsaw.w3.org/css-validator/ found no errors, although CSS validator shows some warnings for using same background  and border color, and for 'unknown' vendor extensions.

Tested on: Win10: Crome80, MS Edge, Firefox 74, Samsung A70, OnePlus 5, Lenovo Yoga Tablet 2 android Chrome. During testing found that the sticky-top funcion does not work on MS Edge and it hold the last position when menu item was clicked, fixed with fixed-top class.

Also found that linux enviroment is case sensitive and had to rename files and folders so it would work on remotely deployed site (github pages), but it worked fie on IONOS linux deployment.

## Known Issues/Bugs

MS Edge smooth-scroll doesn't work.
Map height is not responsive. 

## Feature Change/Left to Implement

Navbar: NA
Home: Split into two categories and create full width-height Hero image
Deals: Simplify banner and add content with HTML and CSS instead on the image and make user controlable carusel
Services: Add 'Find More...' and link to page with more info about the subject.
Testimonials: Add live feed and make as carousel.
Footer: implement postcode, city, email validators. Include T&C, Careers, Policies pages. as for now they are just a placeholders. Make map responsive again. 

## Credits

https://unsplash.com/ - For providing posibility to use images    
https://texe.com/ - For providing posibility to use images     
https://www.w3schools.com - For giving the idea how to solve various issues.
https://getbootstrap.com Bootstrap - for very detailed Documentation     



### Reused Code: 
Link disablement from here : https://css-tricks.com/how-to-disable-links/   
image overlay: https://divinotes.com/overlay-your-images-with-a-pattern-or-translucent-color/
