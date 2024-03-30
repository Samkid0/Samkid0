```html
<!doctype html>
<html>

<head>
    <title>create account</title>
</head>
</colour>blue#0000ff
<body>
    <h1>create account</h1>
    <form id="createaccountform">
        <label for="phone">phone number:</label><br>
        <input type="text" id="phone" name="phone"><br>
        <label for="email">email:</label><br>
        <input type="email" id="email" name="email"><br>
        <label for="password">password:</label><br>
        <input type="password" id="password" name="password"><br>
        <label for="confirmpassword">confirm password:</label><br>
        <input type="password" id="confirmpassword" name="confirmpassword"><br>
        <label for="address">address:</label><br>
        <input type="text" id="address" name="address"><br>
        <label for="invitationcode">invitation code:</label><br>
        <input type="text" id="invitationcode" name="invitationcode"><br>
        <button type="button" onclick="submitform()">done</button>
    </form>

    <div id="accountinfo" style="display: none;">
        <h2>account balance</h2>
        <p>account balance: $1000</p>
        <h2>mining</h2>
        <p>currently mining...</p>
        <h2>euro/dollars chart</h2>
        <img src="chart.png" alt="euro/dollars chart">
        <h2>withdraw</h2>
        <button onclick="withdraw()">withdraw funds</button>
        <h2>send</h2>
        <form id="sendform">
            <label for="receiver">receiver:</label><br>
            <input type="text" id="receiver" name="receiver"><br>
            <button type="button" onclick="send()">send funds</button>
        </form>
    </div>

    <script>
        function submitform() {
            const form = document.getelementbyid('createaccountform');
            const accountinfo = document.getelementbyid('accountinfo');

            form.style.display = 'none';
            accountinfo.style.display = 'block';
        }

        function withdraw() {
            // withdraw logic
            alert('funds withdrawn successfully!');
        }

        function send() {
            // send logic
            alert('funds sent successfully!');
        }
    </script>
</body>

</html>
```



