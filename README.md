<!DOCTYPE html>
<html lang="km">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>គ្រប់គ្រងស្តុក</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>គ្រប់គ្រងស្តុក</h1>

        <!-- 📌 បញ្ចូលស្តុក -->
        <section class="stock-management">
            <h2>បញ្ចូលស្តុក</h2>
            <div class="form-group">
                <input type="text" id="code" placeholder="លេខកូដអីវ៉ាន">
                <input type="text" id="name" placeholder="ឈ្មោះសម្ភារៈ">
                <input type="number" id="price" placeholder="តម្លៃ ($)">
                <input type="number" id="quantity" placeholder="ចំនួន">
                <button id="addProduct">បញ្ចូល</button>
            </div>
            <table>
                <thead>
                    <tr>
                        <th>លេខកូដ</th>
                        <th>ឈ្មោះ</th>
                        <th>តម្លៃ</th>
                        <th>ចំនួន</th>
                        <th>បញ្ចូល</th>
                        <th>បញ្ចេញ</th>
                    </tr>
                </thead>
                <tbody id="productTable"></tbody>
            </table>
        </section>

        <!-- 📌 ប្រវត្តិស្តុក -->
        <section class="stock-history">
            <h2>ប្រវត្តិចេញចូល</h2>
            <table>
                <thead>
                    <tr>
                        <th>កាលបរិច្ឆេទ</th>
                        <th>ឈ្មោះ</th>
                        <th>ប្រភេទ</th>
                        <th>ចំនួន</th>
                    </tr>
                </thead>
                <tbody id="historyTable"></tbody>
            </table>
        </section>

        <!-- 📌 បុងលក់ -->
        <section class="invoice-section">
            <h2>បញ្ជីការលក់</h2>
            <div class="form-group">
                <input type="text" id="sellCode" placeholder="លេខកូដអីវ៉ាន">
                <input type="number" id="sellQuantity" placeholder="ចំនួន">
                <button id="sellProduct">បន្ថែម</button>
            </div>
            <table>
                <thead>
                    <tr>
                        <th>ឈ្មោះអីវ៉ាន</th>
                        <th>ចំនួន</th>
                        <th>តម្លៃ ($)</th>
                        <th>សរុប ($)</th>
                    </tr>
                </thead>
                <tbody id="invoiceTable"></tbody>
            </table>
            <h3>តម្លៃសរុប: <span id="totalAmount">$0.00</span></h3>
            <button id="printInvoice">បោះពុម្ព</button>
        </section>
    </div>

    <script src="script.js"></script>
</body>
</html>
