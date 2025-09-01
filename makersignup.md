---
title: Charnwood Eco Hub Membership Application - Makerspace
layout: single
sitemap: false
header:
  overlay_image: /assets/img/makerspace-banner.png
---

**Thank you for your interest in Charnwood Eco Hub!**

Please complete the application form below to apply for membership of the Charnwood Eco Hub Makerspace. The Charnwood Eco Hub [Library of Things](/projects/library-of-things) and [Scrapstore](/scrapstore) have their own application processes - please see their pages for more information.

<form id="signup_form" method="POST" action="">

<h2>1. Your Details</h2>

<label for="Name">Your Name (required)</label>
<input id="Name" name="Name" type="text" placeholder="Your name" required>
<label for="Phone">Contact Phone Number (required)</label>
<input id="Phone" name="Phone" type="text" placeholder="Your phone number" required>
<label for="Email">Contact Email Addresss</label>
<input id="Email" name="Email" type="email" placeholder="Your email address">
<label for="Membership_Type">Membership Type</label>
<select id="Membership_Type" name="Membership_Type" type="text" required>
<option value="Maker:Indiv">Makerspace: Individual Membership (£15/month)</option>
<option value="Maker:Disc">Makerspace: Student/Low income/Unwaged Membership (£10/month)</option>
</select>
<label for="How_Found">How did you find out about Charnwood Eco Hub?</label>
<select name="How_Found" type="text">
<option value="Leaflet_Poster">Leaflet/Poster</option>
<option value="Website">Website</option>
<option value="Word_of_mouth">Word of mouth</option>
<option value="Social_Media">Social Media</option>
<option value="Other">Other</option>
</select>

<h2>2. Your Interests</h2>

<label for="Interests">Which of the following Makerspace related activities are you interested in? (tick all that apply)</label>
<div><input id="Woodworking" name="Woodworking" type="checkbox"> Woodworking</div>
<div><input id="Metalworking" name="Metalworking" type="checkbox"> Metalworking</div>
<div><input id="Electronics" name="Electronics" type="checkbox"> Electronics</div>
<div><input id="Textiles" name="Textiles" type="checkbox"> Textiles (knitting, sewing etc)</div>
<div><input id="Digital_Fab" name="Digital_Fab" type="checkbox"> Digital Fabrication (3D Printing, laser cutting, CNC milling etc)</div>
<div><input id="Other_Interests" type="checkbox"> Other (please list)</div>
<div><textarea id="Other_Interests_List" name="Other_Interests_List" placeholder="Tell us about any other Makerspace-related interests here"></textarea></div>

<label for="Skills">How would you rate your skill level? (we aim to run workshops to help people develop their skills)</label>
<select id="Skills" name="Skills" type="text">
<option value="Beginner">Beginner</option>
<option value="Intermediate">Intermediate</option>
<option value="Advanced">Advanced</option>
</select>

<h2>3. You And The Makerspace</h2>

<label for="Aspirations">How do you picture yourself using the Makerspace?</label>
<div><input id="Learning" name="Learning" type="checkbox"> Learning how to make and repair</div>
<div><input id="Hobbies" name="Hobbies" type="checkbox"> Working on hobby projects</div>
<div><input id="Professional" name="Professional" type="checkbox"> Professional use</div>
<div><input id="Other_Aspirations" name="Other_Aspirations" type="checkbox"> Other (please list)</div>
<div><textarea id="Other_Aspirations_List" name="Other_Aspirations_List" placeholder="Tell us about other ways you might use the Makerspace here"></textarea></div>

<label for="Volunteering">The Makerspace and the other Eco Hub projects depend on volunteer effort. Would you be interested in volunteering? We have several key roles: </label>
<div><input id="Maintenance" name="Maintenance" type="checkbox"> Maintenance of the equipment and the Makerspace</div>
<div><input id="Teaching" name="Teaching" type="checkbox"> Teaching people how to use the Makerspace</div>
<div><input id="Mentoring" name="Mentoring" type="checkbox"> Mentoring new Makerspace members</div>
<div><input id="Events" name="Events" type="checkbox"> Helping to organise workshops and events</div>
<div><input id="Admin" name="Admin" type="checkbox"> Helping with the day-to-running of the Makerspace</div>
<div><input id="Volunteering_Other" name="Volunteering_Other" type="checkbox">Other volunteering (please list)</div>
<div><textarea id="Volunteering_Other_List" name="Volunteering_Other_List" placeholder="Tell us about other ways you could contribute to the Makerspace / Eco Hub"></textarea></div>

<h2>4. Terms and Conditions</h2>

<div><p>Please note that there is a mandatory induction for new Makerspace members. This is to ensure that everyone understands how to use the equipment safely and what to do in an emergency. As part of this we will also ask you for details of any medical conditions or medication which might affect your use of the Makerspace, and emergency contact information in the event that you should be taken ill.</p></div>
<div><input id="Accepted_Policies" name="Accepted_Policies" value="yes" type="checkbox"> By ticking this box I confirm that I am over 18, and that I accept Charnwood Eco Hub's <a href="/policies">Terms & Conditions and Data Protection Policy</a>.</div>
<div><button type="submit">Submit Your Application</button></div>
</form>

<script type = "text/javascript" >
    window.addEventListener("DOMContentLoaded", function() {
        const yourForm = document.getElementById('signup_form');
        yourForm.addEventListener("submit", function(e) {
            e.preventDefault();
            const data = new FormData(yourForm);
            const action = e.target.action;
            fetch(action, {
                method: 'POST',
                body: data,
            }).then(() => {
                window.location.replace('https://charnwoodecohub.org/makernext')
            })
        })
    });
</script>
