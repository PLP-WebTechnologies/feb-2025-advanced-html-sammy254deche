# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨



(<!DOCTYPE html>
<!-- saved from url=(0032)http://127.0.0.1:5500/index.html -->
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Order List</title>
</head>
<body>
    <section>
        <h2>ordered list</h2>
        <ol type="I">
            <li>First Item</li>
            <li>Second Item</li>
            <li>Third Item</li>
        </ol>
    </section>
    <section>
        <h2>Image</h2>
        <img src="./ASSIGNMENT WEEK 2_files/nature.jpg" alt="The beauty of nature" style="max-width: fit-content; height:auto;">
    </section>

    <section>
        <h2>Contacts</h2>
        <table border="1" cellpadding="5" cellspacing="0">
            <thead>
                <tr>
                    <th>name</th>
                    <th>Address</th>
                    <th>Mobile</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Helen Zawadi</td>
                    <td>567 Tezo St</td>
                    <td>0123547896</td>
                    <td>zawadihelen@gmail.com</td>
                </tr>
                <tr>
                    <td>Alfred Maina</td>
                    <td>678 Mvueni</td>
                    <td>0784521463</td>
                    <td>alfred54@gmail</td>
                </tr>
                <tr>
                    <td>Caleb Kazungu</td>
                    <td>438 Rabai</td>
                    <td>0125436987</td>
                    <td>kazungucaleb@gmail.com</td>
                </tr>
                <tr>
                    <td>Aisha MUhammed</td>
                    <td>890 Bahari</td>
                    <td>0785694235</td>
                    <td>aisha65@gmail.com</td>
                </tr>
                <tr>
                    <td>Mercy Keith</td>
                    <td>0098 Kauma</td>
                    <td>0125436529</td>
                    <td>keithmercy@gmail.com</td>
                </tr>
            </tbody>
        </table>
    </section>

    <section>
        <h2>Registration Form</h2>
        <form action="http://127.0.0.1:5500/index.html#" method="post">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="Enter your name" required=""><br>
            <label for="Email">Email:</label>
            <input type="email" id="Email" name="email" placeholder="Enter your email" required=""><br>
            <label for="password">password:</label>
            <input type="password" id="password" name="password" placeholder="Enter your password" required="" minlength="8"><br>
            <label for="date">Date of Birth</label>
            <input type="date" id="date" name="date" required=""><br>
            <label for="country">country</label>
            <select name="country" id="country" required="">
                <option value="">Select your country</option>
                <option value="Kenya">Kenya</option>
                <option value="Uganda">Uganda</option>
                <option value="Tanzania">Tanzania</option>
            </select><br>

            <p>Gender:</p>
            <label><input type="radio" name="gender" value="male" required=""> Male</label>
            <label><input type="radio" name="gender" value="female"> Female</label>
            <label><input type="radio" name="gender" value="other"> Other</label><br>
            <p>Intrests:</p>
            <label><input type="checkbox" name="intrests" value="sports"> sports</label>
            <label><input type="checkbox" name="intrests" value="music"> Music</label>
            <label><input type="checkbox" name="intrests" value="reading"> Reading</label><br>

            <button type="submit">Register</button>
        </form>
    </section>
<!-- Code injected by live-server -->
<script>
	// <![CDATA[  <-- For SVG support
	if ('WebSocket' in window) {
		(function () {
			function refreshCSS() {
				var sheets = [].slice.call(document.getElementsByTagName("link"));
				var head = document.getElementsByTagName("head")[0];
				for (var i = 0; i < sheets.length; ++i) {
					var elem = sheets[i];
					var parent = elem.parentElement || head;
					parent.removeChild(elem);
					var rel = elem.rel;
					if (elem.href && typeof rel != "string" || rel.length == 0 || rel.toLowerCase() == "stylesheet") {
						var url = elem.href.replace(/(&|\?)_cacheOverride=\d+/, '');
						elem.href = url + (url.indexOf('?') >= 0 ? '&' : '?') + '_cacheOverride=' + (new Date().valueOf());
					}
					parent.appendChild(elem);
				}
			}
			var protocol = window.location.protocol === 'http:' ? 'ws://' : 'wss://';
			var address = protocol + window.location.host + window.location.pathname + '/ws';
			var socket = new WebSocket(address);
			socket.onmessage = function (msg) {
				if (msg.data == 'reload') window.location.reload();
				else if (msg.data == 'refreshcss') refreshCSS();
			};
			if (sessionStorage && !sessionStorage.getItem('IsThisFirstTime_Log_From_LiveServer')) {
				console.log('Live reload enabled.');
				sessionStorage.setItem('IsThisFirstTime_Log_From_LiveServer', true);
			}
		})();
	}
	else {
		console.error('Upgrade your browser. This Browser is NOT supported WebSocket for Live-Reloading.');
	}
	// ]]>
</script>

</body></html>
