---
title: Charnwood Eco Hub Membership Application
layout: single
excerpt: Helping Charnwood to reduce its carbon footprint
header:
  overlay_image: /assets/img/charnwood-eco-hub-banner.jpg
  actions:
    - label: "Donate"
      url: "https://www.paypal.com/donate/?hosted_button_id=V54MWPK2EZGPY"
---

**Thank you for your interest in Charnwood Eco Hub!**

Please complete the application form below to become a member:

<form id="signup_form" method="POST" action="https://script.google.com/macros/s/AKfycbz8VJTh3BdFfmRcEylqbnDtYhunPZwjzPSNqGXBXYI_MPROLEqhNeAzzdGL7VVxzPoMLA/exec">
<label for="Membership_Type">Membership Type</label>
<select name="Membership_Type" type="text" required>
<option value="Scrapstore:Indiv">Scrapstore: Individual/Family membership (£15.00/Yearly)</option>
<option value="Scrapstore:Disc">Scrapstore: Student/Low income/unwaged membership (£10.00/Yearly)</option>
<option value="Scrapstore:Group">Scrapstore: Group membership (£40.00/Yearly)</option>
</select>
<label for="Name">Your Name (required)</label>
<input name="Name" type="text" placeholder="Name" required>
<label for="Address">Your Address (required)</label>
<input name="Address" type="text" placeholder="Address" required>
<label for="Phone">Your Phone Number (required)</label>
<input name="Phone" type="text" placeholder="Phone Number" required>
<label for="Email">Your Email Addresss</label>
<input name="Email" type="email" placeholder="Email Address">
<label for="How_Found">How did you find out about Charnwood Eco Hub?</label>
<select name="How_Found" type="text">
<option value="Leaflet_Poster">Leaflet/Poster</option>
<option value="Website">Website</option>
<option value="Word_of_mouth">Word of mouth</option>
<option value="Social_Media">Social Media</option>
<option value="Other">Other</option>
</select>
<label for="Accepted_Policies" required>By ticking this box I accept Charnwood Eco Hub's Terms & Conditions and Data Protection Policy These are available on-site and on the Charnwood Eco Hub website</label> <input name="Accepted_Policies" type="checkbox">
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
