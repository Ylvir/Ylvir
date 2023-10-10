<!DOCTYPE html>
<html>
<head>
	<title>User Login | HornPub.com</title>
</head>
<body>

		<!--First Name-->
	<p>First name:</p>
	<input type="text" id="FirstName" placeholder="Enter First Name">

		<!--LastName-->
	<p>Last name:</p>
	<input type="text" id="LastName" placeholder="Enter Last Name">

		<!--Age-->
	<p>Age:</p>
	<input type="number" id="AgeNum" placeholder="Enter Age">

		<!--School-->
	<p>School:</p>
	<input type="text" id="SchoolName" placeholder="Enter School Name">
	<br>
	<br>
		<!--button-->
	<button onclick="submit()">Submit</button>

	<br>
		<!--output/result-->
	<p id="Outcome"></p>

	<script>	
		//function
		function submit()
			{
				var FIRSTNAMEElement = document.getElementById("FirstName");
				var LASTNAMEElement = document.getElementById("LastName");
				var AGEElement = document.getElementById("AgeNum");
				var SCHOOLNAMEElement = document.getElementById("SchoolName");
				var OUTCOME = document.getElementById("Outcome");
				
				var firstNameValue = FIRSTNAMEElement.value;
				var lastNameValue = LASTNAMEElement.value;
				var ageValue = parseFloat(AGEElement.value);
				var schoolValue = SCHOOLNAMEElement.value;

				if (firstNameValue == "Johann" && lastNameValue == "Batayen" && ageValue == 18 && schoolValue == "STI WNU") {
					OUTCOME.innerHTML = "Welcome back user!."
				} else
				if (firstNameValue !== "Johann"){
					OUTCOME.innerHTML = "Error! Your are Trying to login into someone's device."
				} else
				if (lastNameValue !== "Batayen"){
					OUTCOME.innerHTML = "Error! Your are Trying to login into someone's device."
				} else
				if (ageValue !== 18){
					OUTCOME.innerHTML = "Error! Your are Trying to login into someone's device."
				} else
				if (schoolValue !== "STI WNU"){
					OUTCOME.innerHTML = "Error! Your are Trying to login into someone's device."
				}

}
						
	</script>

</body>
</html>
