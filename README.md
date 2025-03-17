<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Family Funday - Events in London</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background-color: #f9f9f9;
        }
        header, footer {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 15px;
        }
        .navbar {
            list-style-type: none;
            padding: 0;
            display: flex;
            justify-content: center;
        }
        .navbar li {
            margin: 0 15px;
        }
        .navbar a {
            text-decoration: none;
            color: white;
        }
        .section {
            padding: 20px;
        }
        .payment-section {
            padding: 20px;
            border: 1px solid #ccc;
            max-width: 400px;
            margin: 20px auto;
            background-color: white;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
        }
        input, select, button, textarea {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        button {
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <header>
        <h1>Family Funday! (FamFunday.co.uk)</h1>
        <h2>The site that recommends family-friendly events in London</h2>
        <nav>
            <ul class="navbar">
                <li><a href="#featured">Featured Events</a></li>
                <li><a href="#categories">Event Categories</a></li>
                <li><a href="#contact">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <section id="featured" class="section">
        <h2>Featured Events</h2>
        <!-- Event details -->
    </section>

    <section id="categories" class="section">
        <h2>Event Categories</h2>
        <!-- Category list -->
    </section>

    <section id="contact" class="section">
        <h2>Contact Us</h2>
        <form id="contact-form">
            <div class="form-group">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required />
            </div>
            <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required />
            </div>
            <div class="form-group">
                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="4" required></textarea>
            </div>
            <button type="submit">Submit</button>
        </form>
    </section>

    <section id="payment" class="section">
        <div class="payment-section">
            <h2>Event Booking</h2>
            <div class="form-group">
                <label for="eventSelect">Select Event:</label>
                <select id="eventSelect">
                    <option value="">Choose an event...</option>
                    <option value="christmas">Christmas at Kew (£10/ticket)</option>
                    <option value="robot-zoo">The Robot Zoo (£10/ticket)</option>
                    <option value="imagine">Imagine Festival (£10/ticket)</option>
                </select>
            </div>
            <div class="form-group">
                <label for="numTickets">Number of Tickets:</label>
                <select id="numTickets">
                    <option value="0">Select quantity...</option>
                    <option value="1">1</option>
                    <option value="2">2</option>
                    <option value="3">3</option>
                </select>
            </div>
            <div class="form-group">
                <label>Total Price:</label>
                <div id="priceDisplay">£0.00</div>
            </div>
        </div>
    </section>

    <footer>
        &copy; 2025 Family-Friendly Days Out in London. All Rights Reserved.
    </footer>

    <script>
        const ticketPrice = 10;
        const numTickets = document.getElementById('numTickets');
        const priceDisplay = document.getElementById('priceDisplay');

        numTickets.addEventListener('change', () => {
            const selectedTickets = parseInt(numTickets.value) || 0;
            const total = selectedTickets * ticketPrice;
            priceDisplay.textContent = `£${total.toFixed(2)}`;
        });
    </script>
</body>
</html>
