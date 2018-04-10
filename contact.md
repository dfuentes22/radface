---
layout: default
title: contact
permalink: /contact/
---

<h2 class="page-title">Contact</h2>
<hr>
<p class="page-tagline">Let me know if you'd like to be a model or hire me!</p>
<div class="contact">

	<form action="https://formspree.io/imdanfuentes@gmail.com" method="POST">
		<input type="text" name="name" placeholder="Your Name"><br>
		<input type="email" name="_replyto" placeholder="Your Email"><br>
		<textarea name="message" cols="30" rows="10" placeholder="How can i help you?"></textarea><br>

		<input type="hidden" name="_next" value="{{ site.baseurl }}/thank-you" />
		<input type="hidden" name="_subject" value="Radface New submission!" />
		<input type="text" name="_gotcha" style="display:none" />

		<input type="submit" value="Send">
	</form>

</div>