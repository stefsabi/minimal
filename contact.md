---
layout: default
title: Contact
permalink: /contact/
---

<h1>Contact Me</h1>

<p>If you’d like to get in touch, fill out the form below and I’ll get back to you shortly.</p>

<form action="https://formsubmit.io/send/mrvision@protonmail.ch" method="POST" class="contact-form">
  <input name="_formsubmit_id" type="text" style="display:none"> <!-- spam honeypot -->

  <div class="form-row">
    <div class="form-group">
      <label for="name">First Name</label>
      <input type="text" name="name" required>
    </div>
    <div class="form-group">
      <label for="surname">Last Name</label>
      <input type="text" name="surname" required>
    </div>
  </div>

  <div class="form-group">
    <label for="email">Email</label>
    <input type="email" name="email" required>
  </div>

  <div class="form-group">
    <label for="message">Message</label>
    <textarea name="message" rows="6" required></textarea>
  </div>

  <button type="submit">Get in touch</button>
</form>

<input type="hidden" name="_redirect" value="/thank-you/" />