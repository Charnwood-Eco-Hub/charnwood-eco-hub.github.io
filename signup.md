---
title: Charnwood Eco Hub Membership Application - Scrapstore
layout: single
sitemap: false
header:
  overlay_image: /assets/img/charnwood-eco-hub-banner.jpg
---

**Thank you for your interest in Charnwood Eco Hub!**

Please complete the application form below to apply for membership of the Charnwood Eco Hub Scrapstore. The Charnwood Eco Hub Library of Things has its own application process which is available separately.

<form id="signup_form" class="gform" method="POST" action="https://script.google.com/macros/s/AKfycbznGrjwMz91HIu8LhqD1cYvy_H8Rc6ccdUPRzjq4JlPggbU1i6lqC01ZJRiKHdWpWO3_g/exec">
<label for="Membership_Type">Membership Type</label>
<select id="Membership_Type" name="Membership_Type" type="text" required>
<option value="Scrapstore:Indiv">Scrapstore: Individual/Family/Childminder Membership (£15.00/Yearly)</option>
<option value="Scrapstore:Disc">Scrapstore: Student/Low income/Unwaged Membership (£10.00/Yearly)</option>
<option value="Scrapstore:Group">Scrapstore: Community Groups/Schools Membership (from £40.00/Yearly)</option>
</select>
<label for="Name">Your Name (required)</label>
<input id="Name" name="Name" type="text" placeholder="Your name" required>
<label for="Organisation">Community Group / School (where applicable)</label>
<input id="Organisation" name="Organisation" type="text" placeholder="Your community group or school's name">
<label for="Phone">Contact Phone Number (required)</label>
<input id="Phone" name="Phone" type="text" placeholder="Phone Number" required>
<label for="Email">Contact Email Addresss</label>
<input id="Email" name="Email" type="email" placeholder="Email Address">
<label for="How_Found">How did you find out about Charnwood Eco Hub?</label>
<select name="How_Found" type="text">
<option value="Leaflet_Poster">Leaflet/Poster</option>
<option value="Website">Website</option>
<option value="Word_of_mouth">Word of mouth</option>
<option value="Social_Media">Social Media</option>
<option value="Other">Other</option>
</select>
<div id="container"><input id="Accepted_Policies" class="Accepted_Policies" name="Accepted_Policies" value="yes" type="checkbox" required> <label for="Accepted_Policies">By ticking this box I accept Charnwood Eco Hub's <a href="/policies">Terms & Conditions and Data Protection Policy</a>.</label></div>
<label for="Verify" id="question"></label>
<input id="ans" name="Verify" type="text" placeholder="Please enter the sum of the two numbers here">
<div id="success">Validation complete - you can now submit your Scrapstore application</div>
<div id="fail">Validation failed - something's not quite right, please try again!</div>
<div><button type="submit" id="submit_button">Submit Your Application</button></div>
<div id="lds-ripple" class="lds-ripple"><div></div><div></div></div>
<p id="interstitial" class="interstitial">You should be redirected to the Scrapstore payment page shortly.</p>
</form>

<script type="text/javascript">
    var total;

    function getRandom(){
        return Math.ceil(Math.random()* 20);
    }
    function createSum(){
		var randomNum1 = getRandom(),
			randomNum2 = getRandom();
	    total = randomNum1 + randomNum2;
        $("#question").text("One more thing, I just need to check you aren't a robot. What is " + randomNum1 + " + " + randomNum2 + " ?");
        $("#ans").val('');
        checkInput();
    }

    function checkInput(){
        var input = $("#ans").val(), 
    	slideSpeed = 200, hasInput = !!input, valid = hasInput && input == total;
        $('#message').toggle(!hasInput);
        $('button[type=submit]').prop('disabled', !valid);  
        $('#success').toggle(valid);
        $('#fail').toggle(hasInput && !valid);
    }

    window.addEventListener("DOMContentLoaded", function() {
        const yourForm = document.getElementById('signup_form');
        createSum();
	    $('button[type=reset]').click(createSum);
	    $( "#ans" ).keyup(checkInput);

        yourForm.addEventListener("submit", function(e) {
            e.preventDefault();
            const data = new FormData(yourForm);
            const action = e.target.action;

            var r = document.getElementById("lds-ripple");
            r.style.display = "block";
            r.style.visibility = "visible";

            setTimeout(function(){
            var f = document.getElementById("interstitial");
                f.style.display = "block";
                f.style.visibility = "visible";
            },2000);

            //setTimeout(function(){
            //var f = document.getElementById("interstitial");
            //    f.innerHTML = "
            //},6000);

            fetch(action, {
                method: 'POST',
                body: data,
            }).then(() => {
                window.location.replace('https://charnwoodecohub.org/next-steps')
            })
        })
    });
</script>

