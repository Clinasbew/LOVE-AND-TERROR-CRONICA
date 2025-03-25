<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anonymous Confessions</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            text-align: center;
        }
        textarea {
            width: 100%;
            height: 150px;
            margin: 10px 0;
        }
        button {
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
        .honeypot {
            display: none; /* Hidden field for spam protection */
        }
    </style>
</head>
<body>
    <h1>Submit Your Anonymous Confession</h1>
    <p>Your confession is submitted anonymously. We do not collect any personal information, and your submission is sent directly to the recipient without storing any data.</p>
    <form name="confession-form" method="POST" data-netlify="true" data-netlify-honeypot="bot-field">
        <!-- Honeypot field for spam protection -->
        <input type="text" name="bot-field" class="honeypot">
        <!-- Confession text area -->
        <textarea name="confession" placeholder="Type your confession here..." required></textarea>
        <button type="submit">Submit Confession</button>
    </form>
</body>
</html>
