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


## Step 7: Make the plus/minus button look similar to % (as in iOS calculator app)

Technically, in math the ± character doesn't mean toggling between positive and negative numbers. Designers of the iOS calculator app uses custom character for this purpose, that resembles the % character.


## Step 8: Improve accessibility of the buttons

The plus/minus contains percent character, which will be misleading when used by a user with impaired vision, who uses the calculator with the help of a screen reader. We should add an aria-label to the button to that describes the function of the button. We should also hide the percent character from the screen reader. While we at it, we can also add aria-labels to the other special buttons.


## Step 9: Add event listeners to the number buttons

Let's finally bring life to our app. We'll start by adding event listeners to the number buttons. When a number button is clicked, we want to append the number to the display.


## Step 10: Implement the Clear button

When the Clear button is clicked, we want to clear the display. We will add an event listener to the Clear button to clear the display when it is clicked.


## Step 11: Implement operations

Adding operations makes the calculator more useful. We will add event listeners to the operation buttons to store the operation and the result in the memory. As the operations clicked further, we will calculate the updated result and display it on the screen.


## Step 12: Add the active classes to operations

When an operation is clicked, we want to visually indicate that it is active. We will add an active class to the operation buttons when they are clicked.


## Step 13: Implement the Equal button

When the Equal button is clicked, we want to calculate the result of the operation and display it on the screen. We will add an event listener to the Equal button to calculate the result when it is clicked.


## Step 14: Implement extra use cases of the Equal button

The iOS calculator app has some extra use cases for the Equal button. ... → Equal → Number → Equal should repeat the last operation with the given Number. ... → Equal → Number1 → Operation → Number2 → Equal should perform the operation on the Number1 and Number2, discarding the previous results.


## Step 15: Implement the plus/minus button

When the plus/minus button is clicked, we want to toggle the sign of the number on the display. We will add an event listener to the plus/minus button to toggle the sign of the number when it is clicked. Also, it's time to add some basic formating of the result on the display, so that default hyphen characters would be replaced with correct minus character.


## Step 16: Implement the percent button

In the iOS calculator app, there are two use cases for the percent button. The first use case is to calculate the percentage of the number on the display. The second use case arise in time of operation, where the percent button is used to calculate the percentage of the first number, which is then used in the operation with the second number. We will implement both use cases.


## Step 17: Implement the decimal button

When the decimal button is clicked, we want to add a decimal point to the number on the display. We will add an event listener to the decimal button to add a decimal point to the number when it is clicked.


## Step 18: Handle JavaScript floating point precision issues

JavaScript is a peculiar language in which 0.3 + 0.6 equals to 0.8999999999999999. This is due to the way floating-point numbers are represented in JavaScript. The proper way to fix this is to use the big integer library, but for the sake of simplicity, we will round the results to 10 decimal places.


## Step 19: Limit the number of characters on the display

The iOS calculator app limits the number of characters on the display to 9. We'll do better than that and allow 12 characters on the display. We will add a check to the display to limit the number of characters to 12. Also, we will cut out the extra decimals from the result on big numbers, to make it fit the display. For very large numbers, we display them as exponential after 12 digits.


## Step 20: Fit 12 characters on the display visually

We will add a font-size adjustment to the display to make sure that 12 characters fit on the display. We will also add a transition to the display to make the font-size change more visually appealing.


## Step 21: Add keyboard support

We will add keyboard support to the calculator app. Also, add titles to the buttons to describe their function and explain the keyboard shortcuts.


## Step 22: Highlight buttons triggered with keyboard

When a button is triggered with a keyboard, we want to visually indicate that it is active. We will add an active class to the button when it is triggered with a keyboard.


## Step 23: Add UI scaling so that the calculator looks consistent on mobile devices

The goal is to have the calculator look the same as native app when opened from the mobile device with small screen.