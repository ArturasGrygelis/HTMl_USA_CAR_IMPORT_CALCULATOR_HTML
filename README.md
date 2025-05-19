📦 Car Import & Auction Price Calculator (HTML + CSS for WordPress)
This project is a simple, embedded price calculator for estimating the total cost of car imports from the USA to Lithuania. It includes calculations for:

Auction price

Sea shipping routes

Trucking routes

Destination cities within Lithuania

Additional import-related fees

The calculator is designed to be placed inside a Custom HTML block in a WordPress website.

📋 Features
✅ Pure HTML, CSS, and JavaScript
✅ No external database — all data is embedded via a JSON object inside the HTML code
✅ Dynamic calculation based on user input (car price, selected port, selected city, etc.)
✅ Responsive and lightweight, easily adaptable to any WordPress page

📦 Why JSON in HTML?
Challenge:
WordPress restricts direct access to external JSON or API files from within Custom HTML blocks without extra plugins or PHP custom code.

Solution:
To keep the solution fully contained within the WordPress block editor environment, all shipping, trucking, and city pricing data is stored as a JavaScript JSON object inside the <script> tag in the same HTML file.

This ensures that all calculations are processed client-side, and no external calls are needed.




📁 Project Structure
Since this is a single block of code inside a WordPress Custom HTML block, it follows this structure:

html
Copy
Edit
<div id="calculator">
  <!-- Calculator Form Elements -->
</div>

<style>
  /* CSS Styling for the Calculator */
</style>

<script>
  // JSON Data embedded as JavaScript Object
  const priceData = {
    "ports": { "Newark": 1200, "Houston": 1500 },
    "trucking": { "Los Angeles": 800, "Chicago": 600 },
    "cities": { "Vilnius": 300, "Kaunas": 250 }
  };

  // JavaScript functions for calculation
</script>
🚀 How to Use
Go to your WordPress admin panel

Edit the desired page or post

Add a Custom HTML block

Paste the entire calculator code (HTML + CSS + JavaScript + JSON data)

Save and publish the page

Now, your site visitors can calculate car import prices live on your page.

