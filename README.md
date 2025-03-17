<p>&nbsp;</p>
<p>&nbsp;</p>
<header>
<h1>Family Funday! (FamFunday.co.uk)</h1>
<h2>The site that recommends family-friendly events in London</h2>
<nav>
<ul class="navbar">
<li><a href="#featured">Featured Events</a></li>
<li><a href="#categories">Event Categories</a></li>
<li><a href="#contact">Contact Us</a></li>
<li><a href="#event">Event Booking</a></li>
</ul>
</nav></header>
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
<li><strong>Museums &amp; Exhibitions:</strong> The Robot Zoo, Making Egypt at Young V&amp;A, Wildlife Photography at Natural History Museum.</li>
<li><strong>Theatre &amp; Performances:</strong> Imagine Festival, Back to the Future Musical, The Pea and the Princess at Polka Theatre.</li>
<li><strong>Outdoor Activities:</strong> Christmas at Kew, Land of the Lions at London Zoo.</li>
<li><strong>Workshops &amp; Interactive Events:</strong> Family Freestyle Dance at Sadler&rsquo;s Wells, Art Sundays at Dulwich Picture Gallery.</li>
</ul>
</section>
<div class="payment-section">
    <h2>Event Booking</h2>
    <div class="form-group">
        <label for="eventSelect">Select Event:</label>
        <select id="eventSelect" onchange="updatePrice()">
            <option value="">Choose an event...</option>
            <option value="concert">Christmas at Kew (£10/ticket)</option>
            <option value="conference">The Robot Zoo (£10/ticket)</option>
            <option value="workshop">Imagine Festival (£10/ticket)</option>
        </select>
    </div>
    <div class="form-group">
        <label for="numTickets">Number of Tickets:</label>
        <select id="numTickets" onchange="updatePrice()">
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
    function updatePrice() {
        const eventSelect = document.getElementById('eventSelect');
        const numTickets = document.getElementById('numTickets');
        const priceDisplay = document.getElementById('priceDisplay');
        const ticketPrice = 10; // £10 per ticket

        const selectedEvent = eventSelect.value;
        const selectedTickets = parseInt(numTickets.value) || 0;

        if (selectedEvent && selectedTickets > 0) {
            const total = selectedTickets * ticketPrice;
            priceDisplay.textContent = `£${total.toFixed(2)}`;
        } else {
            priceDisplay.textContent = '£0.00';
        }
    }

    // Initial call to set up the price display
    updatePrice();
</script>
</div>
<!-- Cardholder Name -->
<div class="form-group"><label for="cardholder">Cardholder Name:</label> <input id="cardholder" name="cardholder" required="" type="text" placeholder="Enter your name" /></div>
<!-- Card Number -->
<div class="form-group"><label for="cardnumber">Card Number:</label> <input id="cardnumber" name="cardnumber" required="" type="text" placeholder="1234-5678-9012-3456" /></div>
<!-- Expiry Date -->
<div class="form-group"><label for="expiry">Expiry Date:</label> <input id="expiry" name="expiry" required="" type="month" /></div>
<!-- CVV -->
<div class="form-group"><label for="cvv">CVV:</label> <input id="cvv" name="cvv" required="" type="text" placeholder="123" /></div>
<!-- Submit Button -->
<p><button type="submit">Complete Payment</button></p>



</header>
<h2>Contact Us</h2>
<form id="contact-form"><label for="name">Name:</label><br /> <input id="name" name="name" required="" type="text" /><br /> <label for="email">Email:</label><br /> <input id="email" name="email" required="" type="email" /><br /> <label for="message">Message:</label><br /> <textarea id="message" name="message" required="" rows="4"></textarea><br /> <button type="submit">Submit</button></form></section>



<footer>&copy; 2025 Family-Friendly Days Out in London. All Rights Reserved.</footer>
