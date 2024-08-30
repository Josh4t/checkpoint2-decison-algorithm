// Function to calculate the ticket price based on age.
function calculatePrice() {
    const age = document.getElementById('ageInput').value;
    let priceMessage;

    // Determine the ticket price based on the age entered.
    if (age === '') {
        priceMessage = 'Please enter your age.';
    } else if (age <= 12) {
        priceMessage = 'The ticket price is $10.';
    } else if (age >= 13 && age <= 17) {
        priceMessage = 'The ticket price is $15.';
    } else if (age >= 18) {
        priceMessage = 'The ticket price is $20.';
    } else {
        priceMessage = 'Please enter a valid age.';
    }

    // Display the result in the result paragraph
    document.getElementById('priceOutput').textContent = priceMessage;
}
