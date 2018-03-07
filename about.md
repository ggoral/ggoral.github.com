---
layout: page
title: About me
permalink: /about
---

<img style="width:100%;" src="../img/ggoral.jpg"/>

<span id="years-of-experience"></span> years of experience in open source.

<script>
function timeSince(date) {
  var miliseconds = Math.floor((new Date() - date));
  return Math.floor(miliseconds / 31536000000);
}
var yearsOfExperience = timeSince(new Date('2002-01-01'));
document.getElementById("years-of-experience").innerHTML = yearsOfExperience;
</script>

[jekyll-organization]: https://github.com/jekyll
