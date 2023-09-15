<!DOCTYPE html>
<html>
<head>
    <title>Stationery Store</title>
    <style>
        /* Styles for the webpage */
        /* ... (same as before) ... */
    </style>
</head>
<body>
    <h1>Stationery Store</h1>

    <!-- Pencils section -->
    <h2>Pencils</h2>
    <div>
        <img src="C:\Users\Pratheek\Pictures\Saved Pictures/ps.jpg" alt="Pencil">
        <p>Price: Rs 5</p>
        <p>Available Quantity: <span id="pencil-available">10</span></p>
        <p>Purchase Quantity: <span id="pencil-purchase">0</span></p>
        <input type="number" id="pencil-quantity" name="pencil-quantity" value="0">
        <button type="button" onclick="resetQuantity('pencil-quantity')">Reset</button>
    </div>

    <!-- Erasers section -->
    <h2>Erasers</h2>
    <div>
        <img src="C:\Users\Pratheek\Pictures\Saved Pictures/eraser.jpg" alt="Eraser">
        <p>Price: Rs 3</p>
        <p>Available Quantity: <span id="eraser-available">10</span></p>
        <p>Purchase Quantity: <span id="eraser-purchase">0</span></p>
        <input type="number" id="eraser-quantity" name="eraser-quantity" value="0">
        <button type="button" onclick="resetQuantity('eraser-quantity')">Reset</button>
    </div>

    <!-- Scales section -->
    <h2>Scales</h2>
    <div>
        <img src="C:\Users\Pratheek\Pictures\Saved Pictures/scale.jpg" alt="Scale">
        <p>Price: Rs 5</p>
        <p>Available Quantity: <span id="scale-available">10</span></p>
        <p>Purchase Quantity: <span id="scale-purchase">0</span></p>
        <input type="number" id="scale-quantity" name="scale-quantity" value="0">
        <button type="button" onclick="resetQuantity('scale-quantity')">Reset</button>
    </div>

    <!-- Total Price section -->
    <h2>Total Price: Rs<span id="total-price">0.00</span></h2>

    <!-- Payment button -->
    <button type="button" onclick="calculateTotalPrice()">Payment</button>

    <!-- JavaScript code -->
    <script>
        function calculateTotalPrice() {
            // ... Your existing calculateTotalPrice() function ...

            // Update individual purchase quantities
            document.getElementById("pencil-purchase").textContent = pencilQuantity;
            document.getElementById("eraser-purchase").textContent = eraserQuantity;
            document.getElementById("scale-purchase").textContent = scaleQuantity;
        }

        // ... Your existing functions ...

    </script>
</body>
</html>
