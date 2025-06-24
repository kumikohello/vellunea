---
layout: default
title: Sign Up
---

<h1>Sign Up</h1>

<h2>Join the Email List</h2>
<p>Be the first to know about new releases, shows, and special updates.</p>

<form action="https://buttondown.email/api/emails/embed-subscribe/vellunea" method="post" target="popupwindow" onsubmit="window.open('https://buttondown.email/vellunea', 'popupwindow', 'scrollbars=yes,width=800,height=600,resizable=yes'); return true;">
  <input type="email" name="email" id="bd-email" placeholder="Your email" required style="padding: 10px; margin-right: 10px; border-radius: 4px; border: none; width: 200px;" />
  <input type="submit" value="Subscribe" class="pulse-hover" style="padding: 10px 20px; background-color: var(--accent); color: #1a1a2e; border: none; border-radius: 4px; cursor: pointer;" />
</form>

<p><a href="{{ '/' | relative_url }}" class="back-home pulse-hover">&larr; Back to home</a></p>
