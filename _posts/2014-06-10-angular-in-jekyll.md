---
layout: post
title:  "Angular.js in Jekyll!"
date:   2014-05-07 07:03:47
categories: jekyll update
---

Here is an example of angular.js working in a Jekyll post.

{% assign yourName='{{yourName}}' %}

<div>
<label>Name:</label>
<input type="text" ng-model="yourName" placeholder="Enter a name here">
<hr>
<h1>Hello {{yourName}}!</h1>
</div>

Angular presents us with the problem that its syntax for varibles is the same as Liquid's double curly brackets. To accomdate this we still use the curly brackets in the code, but we add a liquid assign command at the beginning of the body, with the varible equaling the Angular varible with curly brakets between quotation marks. Liquid renders the page happily by swaping its varibles for the angular's syntax and varible as assigned within the Liquid varible. This solution offers no messy javascript and the rendered page as expected with Angular in its normal syntax.

Another way of assigning Liquid varibles is to use the YAML at the top of the Jekyll files and use page.<varible> within the curly brakets; or use the config file and use site.<varible>.


