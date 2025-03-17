<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="styles.css">
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
    <div class="event">
      <h3>Christmas at Kew - 2025</h3>
      <p>Date: November - January</p>
      <p>Location: Kew Gardens</p>
      <p>Description: Enjoy a magical light trail through the gardens, perfect for families during the festive season.</p>
    </div>

    <div class="event">
      <h3>The Robot Zoo</h3>
      <p>Date: August 1st - November 2, 2025</p>
      <p>Location: Horniman Museum</p>
      <p>Description: Explore oversized robotic animals and learn how they mimic real-life creatures.</p>
    </div>

    <div class="event">
      <h3>Imagine Festival</h3>
      <p>Date: Easter Holiday</p>
      <p>Location: Southbank Centre</p>
      <p>Description: A children's literature-themed festival with performances, workshops, and creative activities for ages 0-11.</p>
    </div>

    <div class="event">
      <h3>House of Holi</h3>
      <p>Date: April 8-16, 2025</p>
      <p>Location: Cinnamon Kitchen</p>
      <p>Description: Celebrate Holi with a vibrant paint-throwing experience that's fun for the whole family.</p>
    </div>

    <div class="event">
      <h3>Back to the Future Musical</h3>
      <p>Date: Ongoing</p>
      <p>Location: Adelphi Theatre</p>
      <p>Description: A family-friendly musical adaptation of the iconic movie.</p>
    </div>
  </section>

  <section id="categories" class="section">
    <h2>Event Categories</h2>
    <ul class="categories-list">
      <li><strong>Museums & Exhibitions:</strong> The Robot Zoo, Making Egypt at Young V&A, Wildlife Photography at Natural History Museum.</li>
      <li><strong>Theatre & Performances:</strong> Imagine Festival, Back to the Future Musical, The Pea and the Princess at Polka Theatre.</li>
      <li><strong>Outdoor Activities:</strong> Christmas at Kew, Land of the Lions at London Zoo.</li>
      <li><strong>Workshops & Interactive Events:</strong> Family Freestyle Dance at Sadler’s Wells, Art Sundays at Dulwich Picture Gallery.</li>
    </ul>
  </section>

  <section id="contact" class="section">
    <h2>Contact Us</h2>
    <form id="contact-form">
      <label for="name">Name:</label><br />
      <input type="text" id="name" name="name" required /><br />

      <label for="email">Email:</label><br />
      <input type="email" id="email" name="email" required /><br />

      <label for="message">Message:</label><br />
      <textarea id="message" name="message" rows="4" required></textarea><br />

      <button type="submit">Submit</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Family-Friendly Events in London. All rights reserved.</p>
  </footer>

  <!-- Link to JavaScript -->
  <script src="script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Payment Page - Family-Friendly Days Out in London</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 15px 20px;
            text-align: center;
        }
        main {
            padding: 20px;
        }
        .payment-form {
            background-color: #fff;
            border-radius: 5px;
            padding: 20px;
            max-width: 400px;
            margin: auto;
        }
        .payment-form h2 {
            margin-top: 0;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
        }
        input, select, button {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border-radius: 5px;
            border: 1px solid #ddd;
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
        footer {
            text-align: center;
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
        }
    </style>
</head>
<body>

<header>
    <h1>Complete Your Payment</h1>
</header>

<main>
    <!-- Payment Form -->
    <div class="payment-form">
        <h2>Enter Payment Details</h2>

        <!-- Dummy Payment Form -->
        <form action="#" method="POST">
            
          <!-- Display Event Details -->
          <div class="form-group">
              <label for="event">Selected Event:</label>
              <input type="text" id="event" name="event" value="" readonly>
          </div>

          <!-- Ticket Quantity -->
          <div class="form-group">
              <label for="quantity">Number of Tickets:</label>
              <input type="number" id="quantity" name="quantity" value="" readonly>
          </div>

          <!-- Cardholder Name -->
          <div class="form-group">
              <label for="cardholder">Cardholder Name:</label>
              <input type="text" id="cardholder" name="cardholder" placeholder="Enter your name" required>
          </div>

          <!-- Card Number -->
          <div class="form-group">
              <label for="cardnumber">Card Number:</label>
              <input type="text" id="cardnumber" name="cardnumber" placeholder="1234-5678-9012-3456" required>
          </div>

          <!-- Expiry Date -->
          <div class="form-group">
              <label for="expiry">Expiry Date:</label>
              <input type="month" id="expiry" name="expiry" required>
          </div>

          <!-- CVV -->
          <div class="form-group">
              <label for="cvv">CVV:</label>
              <input type="text" id="cvv" name="cvv" placeholder="123" required>
          </div>

          <!-- Submit Button -->
          <button type="submit">Complete Payment</button>
        </form>
    </div>
</main>

<footer>
    &copy; 2025 Family-Friendly Days Out in London | All Rights Reserved
</footer>

<script>
    // Populate the payment form with event details from query parameters
    const urlParams = new URLSearchParams(window.location.search);
    const event = urlParams.get('event');
    const quantity = urlParams.get('quantity');

    if (event) {
        document.getElementById('event').value = event.replace(/_/g, ' ');
    }

    if (quantity) {
        document.getElementById('quantity').value = quantity;
    }
</script>

</body>
</html>
