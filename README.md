<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IPL PRODUCTS</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #e0f7fa; /* Light green background */
            color: #004d40; /* Dark green text */
            text-align: center;
        }

        .header {
            background-color: #004d40; /* Dark green header */
            color: #ffffff; /* White text */
            padding: 20px;
        }

        .header h1 {
            margin: 0;
        }

        .whats-new {
            font-size: 1.5em;
            color: #ff5722; /* Bright orange color for blinking text */
            animation: blink 1s step-start infinite;
            margin: 20px 0;
        }

        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0; }
        }

        .status-bar {
            background-color: #004d40; /* Dark green status bar */
            color: #ffffff; /* White text */
            padding: 10px;
            overflow: hidden;
            position: relative;
            width: 100%;
            height: 30px;
            line-height: 30px;
        }

        .status-bar span {
            display: inline-block;
            white-space: nowrap;
            padding-left: 100%;
            animation: slide 10s linear infinite;
        }

        @keyframes slide {
            from { transform: translateX(0); }
            to { transform: translateX(-100%); }
        }

        .content {
            padding: 20px;
        }

        .table-container {
            margin: 20px auto;
            width: 90%;
            max-width: 1000px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }

        th, td {
            border: 1px solid #004d40;
            padding: 10px;
            text-align: left;
        }

        th {
            background-color: #004d40;
            color: #ffffff;
        }

        td {
            background-color: #ffffff;
            color: #004d40;
        }

        .editable {
            border: 1px solid #004d40;
            padding: 5px;
            background-color: #ffffff;
            color: #004d40;
            width: 100%;
            box-sizing: border-box;
        }

    </style>
</head>
<body>
    <div class="header">
        <h1>IPL PRODUCTS</h1>
    </div>

    <div class="whats-new">
        WHATS NEW
    </div>

    <div class="status-bar">
        <span>Running Status: All systems are operational and up-to-date with the latest products and updates from IPL.</span>
    </div>

    <div class="content">
        <h2>Welcome to IPL Products</h2>
        <p>Explore our range of IPL products and stay tuned for the latest updates and promotions.</p>
    </div>

    <div class="table-container">
        <table>
            <thead>
                <tr>
                    <th>Column 1</th>
                    <th>Column 2</th>
                </tr>
            </thead>
            <tbody>
                <!-- Generating 20 rows with editable cells -->
                <!-- Using JavaScript to generate rows dynamically -->
                <script>
                    const tableBody = document.querySelector('tbody');
                    for (let i = 0; i < 20; i++) {
                        const row = document.createElement('tr');
                        row.innerHTML = `
                            <td contenteditable="true" class="editable">Row ${i + 1}, Cell 1</td>
                            <td contenteditable="true" class="editable">Row ${i + 1}, Cell 2</td>
                        `;
                        tableBody.appendChild(row);
                    }
                </script>
            </tbody>
        </table>
    </div>
</body>
</html>
