# iOS Calculator App

[This is a part of the Git practice on GitByBit](https://gitbybit.com/) | [Working Demo](https://neochief.github.io/gitbybit-calc/)

For the sake of this practice session, we will try to mimic iOS calculator app with HTML, CSS and JavaScript as close as possible.

We will start by creating a visual representation of the calculator app using HTML and CSS. Then we will add functionality to the calculator using JavaScript.

---


## Step 1: Create the HTML structure

Create a new HTML file and name it `index.html`. Add basic HTML tags to the file.


## Step 2: Add HTML tags for the calculator layout

Add the necessary HTML tags to create the calculator layout. We'll put the buttons in the order they appear in the iOS calculator app. This way we won't have to worry about moving the buttons around later.


## Step 3: Style the calculator layout

For the sake of simplicity, we will be putting our CSS code in the same file as our HTML code.

The calculator itself is centered on the page. The calculator display is at the top, and the buttons are below it. The button layout is a 4x5 grid. We will use CSS Grid to create the layout.


## Step 4: Add CSS classes to the buttons

There are three groups of buttons in the calculator app: numbers, operators, and special buttons. We will add classes to the buttons to differentiate between them. While we at it, we can also add ids to the buttons to make it easier to select them in JavaScript later.


## Step 5: Make the zero button wider

The zero button is wider than the other buttons in the calculator app. We will make the zero button wider by targeting the .b0 class that we added on the previous step.


## Step 6: Style the button groups

Add colors to the button groups to make them visually distinct from each other. We will also add transitions to the button colors to make the hovering and clicking effects more visually appealing. The operator buttons also look better with larger text.