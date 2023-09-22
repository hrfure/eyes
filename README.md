# eyes
Eyes follow cursor program creates a visual effect where two eyeballs continuously follow the mouse cursor's movements


**Overview:**
This simple project creates a visual effect where two eyeballs (balls) follow the movement of the user's cursor on the webpage. As you move your mouse around the webpage, the eyeballs will track and follow its position, giving the illusion that the eyes are watching the cursor.

**HTML Structure:**
The main HTML components are:

A parent container with the class eyes, which houses two individual eyes.
Each eye contains a ball which represents the eyeball that will move according to the cursor's position.
html
Copy code
<div class="eyes">
    <div class="eye">
        <div class="ball"></div>
    </div>
    <div class="eye">
        <div class="ball"></div>
    </div>
</div>
JavaScript Functionality:
The core functionality is provided by the eyes.js script, which contains the following:

Selection of Elements:

The balls constant selects both eyeballs using the class name ball.
Mouse Movement Listener:

An event listener (document.onmousemove) tracks the position of the mouse cursor when it moves.
The clientX and clientY properties of the event object are used to get the X and Y coordinates of the mouse cursor. These values are then converted to percentages relative to the viewport width and height.
For each eyeball (ball), its left and top CSS properties are set to the calculated X and Y percentages, making the balls move with the cursor.
The transform property translates the balls by negative values of the X and Y percentages. This ensures the balls remain within their containing eye elements while following the cursor.
Styling:
Styling is provided by the styles.css stylesheet, which is linked in the HTML header. This stylesheet should define styles for the eyes, eye, and ball classes, determining their size, position, and appearance.

**How to Use:**
Open the HTML file in your web browser.
Move your cursor around the page.
Observe how the eyeballs track and follow the cursor's movement.
Dependencies:
Ensure the following files are in the same directory:

eyes.js: Contains the core JavaScript functionality.
styles.css: Provides the styling for the eyeballs and their containers.

**How to Improve:**
Add eyelids that blink at regular intervals or whenever the user clicks.
Add a gradient or shadow to the eyeballs for a more 3D look.
Implement a boundary for the eyeball movement so they don't exit the eye container.
