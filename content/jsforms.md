---
title: "Client side validation with HTML5 -Godsgift Akari"
date: 2019-09-14T14:46:10+06:00
description: "JavaScript Client side validation"
type: "post"
image: "custom_images/Gift_Akari_Profile.png"
categories:
  - "JavaScript"
tags:
  - "Web"
  - "Software"
---

### Client-side form validation with HTML5

For a good user experience, beefore submitting form data to the server for processing , it is important to ensure required form data are filled in and correctly too. Client-side form validation helps ensure data submitted matches the requirements set forth in the various form controls saving the trip to the server for each common task.

```js
// post method is used to send the form to the server
<form action="/thankyou.js" method="post">
  <input type="text" name="firstName" required>
  <input type="submit" value="Submit">
</form>


```

The code above assumes that **/thankyou.js** is the server-side file to send to the user when the form is submitted.
