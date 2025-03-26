// script.js

// Get elements
const envelope = document.getElementById("envelope");
const letter = document.getElementById("letter");
const clickButton = document.getElementById("clickButton");

// Add event listener for envelope click
envelope.addEventListener("click", () => {
    // Show the letter and button after envelope click
    envelope.classList.add("show-envelope");
    letter.classList.add("show-letter");

    // Display the 'Click here' button
    setTimeout(() => {
        clickButton.style.display = "block";
    }, 1500); // Delay button appearance after animation
});

// Add functionality for the button to navigate to another page
clickButton.addEventListener("click", () => {
    window.location.href = "https://yourwebsite.com/another-page"; // Change this URL to your actual destination
});
