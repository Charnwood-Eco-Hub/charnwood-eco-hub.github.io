---
title: Charnwood Eco Hub Membership Application - Scrapstore
layout: single
sitemap: false
header:
  overlay_image: /assets/img/charnwood-eco-hub-banner.jpg
  actions:
    - label: "Donate"
      url: "https://www.paypal.com/donate/?hosted_button_id=V54MWPK2EZGPY"
---

**Thank you for your interest in Charnwood Eco Hub!**

Please complete the application form below to apply for membership of the Charnwood Eco Hub Scrapstore. The Charnwood Eco Hub Library of Things has its own application process which is available separately.

<form id="signup_form" method="POST" action="https://script.google.com/macros/s/AKfycbznGrjwMz91HIu8LhqD1cYvy_H8Rc6ccdUPRzjq4JlPggbU1i6lqC01ZJRiKHdWpWO3_g/exec">
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
<label for="Email">Contact Email Addresss (required)</label>
<input id="Email" name="Email" type="email" placeholder="Email Address">
<label for="How_Found">How did you find out about Charnwood Eco Hub?</label>
<select name="How_Found" type="text">
<option value="Leaflet_Poster">Leaflet/Poster</option>
<option value="Website">Website</option>
<option value="Word_of_mouth">Word of mouth</option>
<option value="Social_Media">Social Media</option>
<option value="Other">Other</option>
</select>
<label for="Accepted_Policies" required>By ticking this box I accept Charnwood Eco Hub's <a href="/policies">Terms & Conditions and Data Protection Policy</a>.</label><input id="Accepted_Policies" name="Accepted_Policies" value="yes" type="checkbox">
<div id="foo">
<p>
</p>
</div>
<button type="submit">Submit Your Application</button>
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
                window.location.replace('https://charnwoodecohub.org/next-steps')
            })
        })
    });
</script>
