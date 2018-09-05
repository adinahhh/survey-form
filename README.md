# survey-form

<head>
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="https://fonts.googleapis.com/css?family=Montserrat" rel="stylesheet">
	<script src="https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js"></script>
</head>
<!--Begin form content here -->

<h1 id="title">Survey Form</h1>
<p id="description">Please complete this survey.</p>
<p>
<form id="survey-form" action="/submit-survey-form">
  <label for="choose" id="name-label">* Your name:</label>
<input type="text" placeholder="Enter your name" id="name" required pattern="[A-za-z\s ]+">
  </p>
  <p>
  <label for="choose" id="email-label">* Your email:</label>
  <input type="email" id="email" placeholder="Enter your email" required>
  </p>
  <p>
  <label for="number" id="number-label">* Your phone number:</label>
  <input type="number" placeholder="Enter your number" min="10" max="10" id="number" required>
  </p>

<!--Begin radio buttons here -->

<p>Please select your preferred contact method:</p>
<div>
    <input type="radio" id="contactChoice1" name="contact" value="email">Email 
    <input type="radio" id="contactChoice2"
     name="contact" value="phone">Phone
</div>

<p>
  <label for="realtor">Are you working with a realtor?
  <input type="radio" name="realtor" value="1">Yes
  <input type="radio" name="realtor" value="2">No
    </label>
         </p>
<p>
  <label for="loan">Have you received a loan preapproval?</label>
  <input type="radio" name="preapproval" value="yes">Yes
  <input type="radio" name="preapproval" value="no">No
  </label>
</p>
<p>
  <label>What is your pricepoint?</label>
<select name="pricepoint" id="dropdown">
<option value="under 200k">under 200k</option>
<option value="200-300k">200-300k</option>
<option value="300-450k">300-450k</option>
<option value="450-600k">450-600k</option>
<option value="600k+">600k+</option>
</select>
</p>

<!-- start checkboxes -->
<label>What are important factors when buying your new home? </label>
<div>
  <input type="checkbox" name="factors" value="schools">School district
  <input type="checkbox" name="factors" value="floor">Open floor plan
  <input type="checkbox" name="factors" value="backyard">Backyard size
  <input type="checkbox" name="factors" value="pool">Pool
</div> 
  <p>
    <label>Any comments or questions?</label>
    <textarea placeholder="Enter comments here" rows="2" cols="25" maxlength="150"></textarea>
      </p>

  <button type="submit" id="submit">Submit</button>
</form>
<br>
<footer>This form was completed as a project for FreeCodeCamp.</footer>
