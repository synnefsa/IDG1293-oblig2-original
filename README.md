[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WMNqWEYY)
[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=18907824)
# IDG1293-2025-oblig2

This document contains the description for the second compulsory assignment of the course IDG1293.

# Goal

* Prove knowledge and understanding of SVGs, SVGs animations, CSS drawing, and CSS animations.
* Implement a poster design using HTML and CSS, preserving aspect ratio and ensuring responsiveness.
* Use SVGs and CSS drawing to animate parts of the poster for enhanced visual appeal.
* Encourage creativity and innovation in web design.
* Practice SASS.
* Understand and apply concepts of Modular Scales and Fluid Typography to create visually harmonious and adaptable text designs.

# Introduction

**Scenario**

Digital sustainability is becoming increasingly important in today's world. NTNU has created a series of posters promoting digital sustainability, available in PDF format [here](https://www.ntnu.no/design/digital-barekraft/illustrasjoner). These posters are visually appealing for children and contain various elements that can be animated to create engaging web experiences.

# Context

In this "oblig" you will be presented with a brief description of the problem you have to solve. Have in mind the [Goal section](#Goal) when you design and implement your assignment. 

This is **an individual task**, and you are required to build everything from the ground up. Although, you may utilize snippets of code from tutorials or official documentation, you must clearly acknowledge the sources in the comments of your code. Plagiarism or cheating will be deemed to have taken place if the submitted code shows substantial similarities to other students' assignments or projects found online. In such cases, the matter will be reported to the NTNU appeals committee for further examination. If you have any doubts regarding the use of materials for your project, please reach out to the instructor for clarification. 

It is imperative to deliver the assignment within the set deadline (never after).

# Task
For this task, you are presented with two options. **Option 1** is the default and preferred choice, designed to guide you through a structured and well-defined implementation process. **Option 2** is an alternative for those who have a **unique and ambitious idea of similar complexity** to Option 1. This allows you the flexibility to explore/design a concept/poster you feel passionate about while maintaining the same level of challenge.

## Option 1: Structured Implementation
This option provides a clear framework for completing the assignment. You will:
1. Work with the specific poster provided to all students [Webben og planeten vår](https://www.ntnu.no/documents/10401/0/web_poster1.pdf/ef46a3c3-6a8a-1c59-1f3a-d3f73713ec17?t=1695296028666).
    - Use software like Adobe Illustrator to extract elements from the poster.
    - Ensure that the extracted elements preserve the aspect ratio and are suitable for web implementation.
    - Optimise or rewrite the elements when needed.
2. Implement the poster design using HTML and CSS, ensuring responsiveness and aspect ratio preservation.
3. Animate key elements of the poster using SVGs, CSS animations, and other techniques.
4. Document your process and decisions in `documents/report.md`.

## Option 2: Creative Exploration
If you have a unique idea that aligns with the assignment's goals and complexity, you may choose this option. Your idea must:
1. Be approved by the instructor before implementation. To apply, send an email to Carlos with the subject line: **"IDG1293 oblig 2 - alternative idea"**. Include the following in your email:
    - A mockup of your idea.
    - A detailed explanation of your concept and why it aligns with the assignment's goals.
    - A plan outlining the techniques and animations you will use, demonstrating how your idea matches the complexity and requirements of Option 1.
    - Check Blackboard to see the deadline to submit your idea. If the suggestion is not submited before the deadline, then you will have to work with Option 1.
2. Demonstrate equivalent knowledge and skills in SVGs, CSS animations, and responsive design.
3. Include animations and interactions that showcase creativity and technical proficiency.
4. Be thoroughly documented in `documents/report.md`, explaining your approach and how it meets the assignment's objectives.

Regardless of the option you choose, ensure that your work adheres to the guidelines and requirements outlined in this document and during the lectures.

## Task (regardless of option)

1. **Choose an option**: By default, implement Option 1. If you prefer Option 2, submit an application to Carlos for approval (see [Option 2](#option-2-creative-exploration)).

2. **Implement poster design**:
    - Implement the poster design using HTML and CSS.
    - Ensure responsiveness and preserve the aspect ratio of the poster.

3. **Animate poster elements**:
    - Identify the primary illustrations suitable for animation, specifically selecting those that can demonstrate a good knowledge in various types of animations, including CSS animations, SMIL path animations, SMIL animate, and SMIL transform. Optionally, consider including GSAP animations.
    - Ensure that animated elements are incorporated into all sections of the posters to provide a comprehensive showcase of animation techniques.
    - Utilize SVGs and CSS drawing techniques to animate parts of the poster.
    - Enhance the visual appeal of the poster by adding animations that bring elements to life.
    - Aim for smooth transitions and engaging visual effects.

4. **Interactions (Optional)**:
    - While interactions with elements are allowed, focus on creating animations that enhance the poster's visual impact even without user interactions.
    - Experiment with hover effects, click interactions, etc., if time allows and if they contribute positively to the overall design.

5. **Documentation**:
    - Edit `documents/report.md` to explain your process and list all the elements you have animated, the type of animation you have used for each type and the reason why you used that type.

# Folder Structure

- `README.md`: This document describing the assignment.
- `index.html`:  Base HTML file with a predefined structure. Students must implement their poster design inside the #poster-container element.
- `assets/`: Folder containing extracted elements from the chosen poster (if needed).
- `assets/styles/styles.scss`: SCSS file containing styles for the poster design and animations.
- `assets/styles/poster.css`: CSS file containing core poster layout styles, viewport handling, fullscreen mode, and print media queries. NOTE: You are not allowed to edit this file. 
- `assets/scripts/poster.js`: JavaScript file handling poster display modes, viewport transitions, and width calculations. NOTE: You are not allowed to edit this file.
- `misc/github-pages.pdf`: pdf file with instructions to deploy project in GitHub pages.
- `documents/report.md`: Document outlining the steps took during implementation.

# Testing

Before submitting your assignment, ensure thorough testing of your poster implementation:

1. **Viewport Testing**:
   - Test the poster in both viewport-fit and fullscreen modes using the "Toggle Fullscreen" button
   - Verify that all elements maintain their relative positions and proportions
   - Check that animations remain smooth during transitions between modes

2. **Responsive Testing**:
   - Test the poster at different viewport sizes by resizing your browser window
   - Ensure all SVG elements scale properly without distortion
   - Verify that text remains readable at all sizes
   - Check that animations work correctly at different scales

3. **Animation Testing**:
   - Verify that all animations play as intended
   - Check that animations don't interfere with each other
   - Test that animations restart properly when switching between viewport modes

4. **Cross-browser Testing**:
   - Test the poster in different modern browsers (Chrome, Firefox, Safari)
   - Verify that all SVG animations and CSS effects work consistently

5. **Print Preview**:
   - Check how the poster looks in print preview mode (test A4 and A3 formats).
   - Ensure all elements are visible and properly positioned when printed.

# Delivery

This assignment must be delivered in three different places: GitHub classroom, Github pages and Blackboard. The project must also be deployed in GitHub pages.

**GitHub Classroom**
* To deliver the assignment in GitHub Classroom, you only need to make sure all your changes and commits are pushed to your Git repository.
    * A Pull request is created automatically when the repository is cloned. Feedback will be included there if needed. Do not remove or close that Pull Request.
    * Only the changes in the "main" branch will be considered the final version. Do not close the other branches since we will look how you have collaborated using Git.

* It is imperative that you work exclusively with this Git repository to ensure that all modifications are trackable and your code is backed up on a regular basis. Hence, you should commit your progress directly to this repository each time you make advancements.

**GitHub Classroom**

* Follow the instructions found in `misc/github-pages.pdf`.

**Blackboard**

* Before delivering the assignment in Blackboard, make sure your project has all the files it needs. Delete any file, folder or info that is not needed (e.g.: `.git/` folder). Zip the project and upload the file to Blackboard.
