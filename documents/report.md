# Report

## Introduction
The objective of this assignment was to implement an existing poster design using HTML, CSS and SVG animations while also ensuring responsiveness and preserving aspect ratio. The design needed to implement various animation techniques, including CSS animations, SMIL and optionally GSAP. 

## Content
### Sections
The poster was divided into three main sections in the html: each including roughly 1/3 of the page each with their corresponding text and illustrations. This was to get a simple and clear "overview" of the poster. Each section includes a background color (light blue, dark blue and pink) with their corresponding text and illustrations. 


### Fonts
I used Adobe Illustrator to trace the fonts and found that it most likely is used Open Sans Semibold and Extrabold from Google Fonts, as well as Marydale Bold from Adobe fonts. 

### Adobe Illustrator and SVG Elements
I used Adobe Illustrator to extract the poster's graphical elements. After a lot of fiddling with a program I am not confident in, I managed to extract the main illustrations as SVG files, so I could later animate these elements in CSS and HTML. I extracted parts that I thought it would be fun to animate, for example the different elements such as sun, cloud, earth, characters etc. 
Additionally, I extracted the background colors as one SVG element: the organic forms in light blue, dark blue and pink. To have more control over the layering, in case I wanted to change it, I extracted the part with the lines as an "overlay" on the background. I intended to add the footer manually as well, but I did noot quite finish it in time, therefore, it is commented out for now. In the images folder, I have both the background without and with the footer, as well as the SVG for the footer background, to finish it later. 

## Animations
### CSS Keyframe
I implemented CSS animations for many of the svg elements using @keyframe. I have used different animations like translate, rotate and scale to showcase different animation styles. They have smooth transitions and can create cool visual effects. 

### SMIL and GSAP
When opening the svg elements, the html code for the svg's are provided so I could apply SMIL animation for some of the elements. However, I read that Safari does not support all SMIL animations, but it works in my Google Chrome. I therefore also tried to implement GSAP animation for one element, which is the green arrow at the top. Since I only applied it to one element, I did not make an external script for it, and I placed the internal script it at the bottom of the body in a script tag.
I used SMIL animation for the growing eyes on the earth, where I used animateTransform and scaling. I also used animateTransform with translate for the small cloud to go up and down. Lastly, I used the animateMotion for the little green bacteria to follow a path (circle). 
Sources for inspiration: 
- https://css-tricks.com/guide-svg-animations-smil/
- https://developer.mozilla.org/en-US/docs/Web/SVG/Guides/SVG_animation_with_SMIL


## Responsiveness 
### Typography and positioning
I used flexible units like percentages and viewport units to ensure that the elements were resized proportionally and aligned with the original poster. To address different screen sizes, I implemented fluid typography with the CSS clamp()-function. This was intended to ensure that the text was readable on small screens and that the text scales correctly. However, I faced some challenges with the scaling on large screens despite trying to use the clamp() function. The text became either too small on larger screens or too large on smaller screens. It seemed that the clamp()-function was not offering the control I needed and I found it hard to balance the text on small and large screens.

I found it a bit challenging to understand and implement the idea of scaling a poster layout in this way. Since posters are typically fixed in size, it felt a bit unusual to make it responsive using clamp() and flexible units. While they are meant to help with scalability, I did not feel that the behavior was always consistent across screen sizes. I ended up with a version that looks good on medium and smaller screens, and works fine — though not as good as I wanted it to be — on larger ones.


### Testing
I have tested the poster in both viewport-fit and fullscreen modes using the "toggle fullscreen" button, and all elements maintain their positions, and animations remain smooth. Typography stays readable because of the clamp() function, however, it could have scaled a bit better, especially on larger screens. Animations works as expected in Google Chrome, but SMIL animations did not run in Safari, which probably is based on browser support limitations and my version of Safari. 


## Conclusion
I think this poster design fulfills the criteria for the assignment, and incorporates different types of animations, from CSS Keyframe to SMIL and GSAP. I also think that using percent for scaling worked good for keeping elements in their positions when toggling between screen sizes. 

## CREDITS
Fonts: 
- [https://fonts.adobe.com/fonts/marydale](https://fonts.adobe.com/fonts/marydale)
- [https://fonts.google.com/specimen/Open+Sans?preview.text=Whereas%20recognition%20of%20the%20inherent%20dignity](https://fonts.google.com/specimen/Open+Sans?query=open+sans)