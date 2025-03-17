<!DOCTYPE html>
<html>
<head>
    <title>Event Booking System</title>
    <style>
        .payment-section {
            padding: 20px;
            border: 1px solid #ccc;
            max-width: 400px;
            margin: 20px auto;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
        }
        select, #priceDisplay {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ddd;
        }
    </style>
</head>
<body>
    <div class="payment-section">
        <h2>Event Booking</h2>
        
        <div class="form-group">
            <label for="eventSelect">Select Event:</label>
            <select id="eventSelect">
                <option value="">Choose an event...</option>
                <option value="concert">Summer Concert (£10/ticket)</option>
                <option value="conference">Tech Conference (£10/ticket)</option>
                <option value="workshop">DevOps Workshop (£10/ticket)</option>
            </select>
        </div>

        <div class="form-group">
            <label for="numTickets">Number of Tickets:</label>
            <select id="numTickets">
                <option value="0">Select quantity...</option>
                <option value="1">1</option>
                <option value="2">2</option>
                <option value="3">3</option>
                <option value="4">4</option>
                <option value="5">5</option>
                <option value="6">6</option>
            </select>
        </div>

        <div class="form-group">
            <label>Total Price:</label>
            <div id="priceDisplay">£0.00</div>
        </div>
    </div>

    <script>
        // Price calculation logic
        const ticketPrice = 10; // £10 per ticket
        const numTickets = document.getElementById('numTickets');
        const priceDisplay = document.getElementById('priceDisplay');

        numTickets.addEventListener('change', calculateTotal);

        function calculateTotal() {
            const selectedTickets = parseInt(numTickets.value) || 0;
            const total = selectedTickets * ticketPrice;
            priceDisplay.textContent = `£${total.toFixed(2)}`;
        }

        // Initial calculation
        calculateTotal();
    </script>
</body>
</html>
