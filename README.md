
 <!DOCTYPE html>
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
         <li><a href="#contact">Complete Your Payment</a></li>
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
     <title>Event Booking System</title>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Family Funday - Events in London</title>
     <link rel="stylesheet" href="styles.css">
     <style>
         .payment-section {
             padding: 20px;
             border: 1px solid #ccc;
             max-width: 400px;
             margin: 20px auto;
         body {
             font-family: Arial, sans-serif;
             margin: 0;
             background-color: #f9f9f9;
         }
         .form-group {
             margin-bottom: 15px;
         header, footer {
             background-color: #4CAF50;
             color: white;
             text-align: center;
             padding: 15px;
         }
         label {
             display: block;
             margin-bottom: 5px;
         .navbar {
             list-style-type: none;
             padding: 0;
             display: flex;
             justify-content: center;
         }
         select, #priceDisplay {
             width: 100%;
             padding: 8px;
             margin-bottom: 10px;
             border: 1px solid #ddd;
         .navbar li {
             margin: 0 15px;
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
                 <option value="concert">Christmas at Kew (£10/ticket)</option>
                 <option value="conference">The Robot Zoo (£10/ticket)</option>
                 <option value="workshop">Imagine Festival (£10/ticket)</option>
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
         .navbar a {
             text-decoration: none;
             color: white;
         }
 
         // Initial calculation
         calculateTotal();
     </script>
 </body>
 </html>
 
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
 <header>
     <h1>Complete Your Payment</h1>
 </header>
 
 <main>
 
 </body>
 </html>
 
       .payment-form {
             background-color: #fff;
             border-radius: 5px;
         .section {
             padding: 20px;
             max-width: 400px;
             margin: auto;
         }
         .payment-form h2 {
             margin-top: 0;
         .payment-section {
             padding: 20px;
             border: 1px solid #ccc;
             max-width: 400px;
             margin: 20px auto;
             background-color: white;
         }
         .form-group {
             margin-bottom: 15px;
 @@ -216,12 +47,12 @@
             display: block;
             margin-bottom: 5px;
         }
         input, select, button {
         input, select, button, textarea {
             width: 100%;
             padding: 8px;
             margin-bottom: 10px;
             border-radius: 5px;
             border: 1px solid #ddd;
             border-radius: 5px;
         }
         button {
             background-color: #4CAF50;
 @@ -232,58 +63,93 @@
         button:hover {
             background-color: #45a049;
         }
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
 
         footer {
             text-align: center;
             padding: 10px 20px;
             background-color: #4CAF50;
             color: white;
         }
     </style>
 </head>
 <body>
  <footer>
     <p>&copy; 2025 Family-Friendly Events in London. All rights reserved.</p>
   </footer>
     <header>
         <h1>Family Funday! (FamFunday.co.uk)</h1>
         <h2>The site that recommends family-friendly events in London</h2>
         <nav>
             <ul class="navbar">
                 <li><a href="#featured">Featured Events</a></li>
                 <li><a href="#categories">Event Categories</a></li>
                 <li><a href="#contact">Contact Us</a></li>
                 <li><a href="#payment">Complete Your Payment</a></li>
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
 
   <!-- Link to JavaScript -->
   <script src="script.js"></script>
         numTickets.addEventListener('change', () => {
             const selectedTickets = parseInt(numTickets.value) || 0;
             const total = selectedTickets * ticketPrice;
             priceDisplay.textContent = `£${total.toFixed(2)}`;
         });
     </script>
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
