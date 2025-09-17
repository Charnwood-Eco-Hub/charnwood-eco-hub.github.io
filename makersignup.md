---
title: Charnwood Eco Hub Membership Application - Makerspace
layout: single
sitemap: false
header:
  overlay_image: /assets/img/makerspace-banner-dim.png
---

**Thank you for your interest in Charnwood Eco Hub!**

Please complete the application form below to apply for membership of the Charnwood Eco Hub Makerspace. The Charnwood Eco Hub [Library of Things](/projects/library-of-things) and [Scrapstore](/scrapstore) have their own application forms - please see their pages for more information.

<form id="signup_form" class="gform" method="POST" action="https://script.google.com/macros/s/AKfycbzIWYEScB1boqm9UOBf3bY1zsBfyuyA3ECBeI7mKXFBsd_ZURiNoBm5G-ICs2GPMp_eOQ/exec">

<h1>About You</h1>

<div><p>Your Name (required)<br/>
<input id="Name" name="Name" type="text" placeholder="Your name" required><br/>
Contact Phone Number (required)<br/>
<input id="Phone" name="Phone" type="text" placeholder="Your phone number" required><br/>
Contact Email Addresss<br/>
<input id="Email" name="Email" type="email" placeholder="Your email address">
Membership Type<br/>
<select id="Membership_Type" name="Membership_Type" type="text" required>
<option value="Maker:Indiv">Makerspace: Individual Membership (£15/month)</option>
<option value="Maker:Disc">Makerspace: Student/Low income/Unwaged Membership (£10/month)</option>
</select>
How did you find out about the Makerspace?<br/>
<select name="How_Found" type="text">
<option value="UNKNOWN">Please pick one</option>
<option value="Leaflet_Poster">Leaflet/Poster</option>
<option value="Website">Website</option>
<option value="Word_of_mouth">Word of mouth</option>
<option value="Social_Media">Social Media</option>
<option value="Other">Other</option>
</select>
</p></div>

<h1>Your Interests</h1>

<div><p>We'd like to learn more about what makes people interested in the Makerspace. If you're OK with that, tick the boxes to let us know which of the following you're interested in:
<ul>
<li><input id="Woodworking" name="Woodworking" type="checkbox"> <label for="Woodworking">Woodworking</label></li>
<li><input id="Metalworking" name="Metalworking" type="checkbox"> <label for="Metalworking">Metalworking</label></li>
<li><input id="Electronics" name="Electronics" type="checkbox"> <label for="Electronics">Electronics</label></li>
<li><input id="Textiles" name="Textiles" type="checkbox"> <label for="Textiles">Textiles - knitting, sewing etc</label></li>
<li><input id="Digital" name="Digital" type="checkbox"> <label for="Digital">Digital Fabrication - 3D Printing, laser cutting, CNC milling etc</label></li>
</ul>
</p>
</div>

<div><p>Other Interests
<textarea id="Other_Interests" name="Other_Interests" placeholder="Perhaps you have some other Makerspace-related interests that aren't on our list? You can tell us about them here if you want to."></textarea>
How would you rate your skill level?<br/>
<select id="Skills" name="Skills" type="text">
<option value="UNKNOWN">Please pick one</option>
<option value="Beginner">Beginner</option>
<option value="Intermediate">Intermediate</option>
<option value="Advanced">Advanced</option>
</select><br/>
By the way, you don't have to be an expert to use the Makerspace - it's for everyone, and beginners are very welcome. We run regular workshops to help people develop their skills.</p></div>

<h1>What Will You Make?</h1>

<div><p>How do you picture yourself using the Makerspace?<br/>
<ul>
<li><input id="Learning" name="Learning" type="checkbox"> <label for="Learning">Learning how to make and repair</label></li>
<li><input id="Hobbies" name="Hobbies" type="checkbox"> <label for="Hobbies">Working on hobby projects</label></li>
<li><input id="Professional" name="Professional" type="checkbox"> <label for="Professional">Professional use</label></li>
</ul>
</p></div>

<div><p>Other Makerspace Uses
<textarea id="Other_Uses" name="Other_Uses" placeholder="Maybe you have a particular project you'd like to work on at the Makerspace? We'd love to know more - tell us about it here!"></textarea></p></div>

<h1>Volunteering Opportunities</h1>

<div><p>The Makerspace and the other Eco Hub projects depend on volunteer effort. We'd love to have you onboard if you are interested in volunteering.</p>
<p>There are lots of ways you could help out. Tick the boxes if you see any you're interested in:
<ul>
<li><input id="Maintenance" name="Maintenance" type="checkbox"> <label for="Maintenance">Maintenance of the equipment and the Makerspace</label></li>
<li><input id="Teaching" name="Teaching" type="checkbox"> <label for="Teaching">Teaching people how to use the Makerspace</label></li>
<li><input id="Mentoring" name="Mentoring" type="checkbox"> <label for="Mentoring">Mentoring new Makerspace members</label></li>
<li><input id="Events" name="Events" type="checkbox"> <label for="Events">Helping to organise workshops and events</label></li>
<li><input id="Admin" name="Admin" type="checkbox"> <label for="Admin">Helping with the day-to-running of the Makerspace</label></li>
</ul>
</p></div>

<div><p>Other Volunteering Ideas
<textarea id="Volunteering_Other" name="Volunteering_Other" placeholder="Maybe you have some other ideas about how you could support the Makerspace / Eco Hub? Tell us about them here."></textarea></p></div>

<h1>Terms and Conditions</h1>

<div><p>Please note that there is a mandatory induction for new Makerspace members. This is to ensure that everyone understands how to use the equipment safely and what to do in an emergency.</p></div>
<div><p>As part of this we will also ask you for details of any medical conditions or medication which might affect your use of the Makerspace, and emergency contact information in the event that you should be taken ill.</p></div>
<div><p><input id="Accepted_Policies" class="Accepted_Policies" name="Accepted_Policies" value="yes" type="checkbox" required> <label for="Accepted_Policies">By ticking this box I confirm that I am over 18, and that I accept Charnwood Eco Hub's <a href="/policies">Terms & Conditions and Data Protection Policy</a>.</label></p></div>
<div><p><button type="submit">Submit Your Application</button></p></div>
<div id="lds-ripple" class="lds-ripple"><div></div><div></div></div>
<p id="interstitial" class="interstitial">You should be redirected to the Makerspace payment page shortly.</p>
</form>

<script type = "text/javascript" >
    window.addEventListener("DOMContentLoaded", function() {
        const yourForm = document.getElementById('signup_form');
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
                window.location.replace('https://charnwoodecohub.org/makernext')
            })
        })
    });
</script>
