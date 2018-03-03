---
layout: post
title: tips4myfirsthouse
thumbnail-path: "img/tips.png"
short-description: Custom page for local real state agent

---

{:.center}
![]({{ site.baseurl }}/img/tips.png)
<h3><a href ="http://www.tips4myfirsthouse.com/">Go To tips4myfirsthouse</a></h3>

## Explanation

tips4myfirsthouse was my first freelance client. I am continuing to work with my client to customize his website.
It uses rails on the backend with mostly Bootstrap on the front end. We created a custom site that would make purchasing a home easier for future home buyers. I am using the ActiveAdmin gem for him to have access to the emails for his potential clients.

## Problem

I needed the site to be a responsive design to run on every platform we could manage. That means that www.tips4myfirsthouse needed to adapt to the user’s device such as desktop, tablet, or smartphone, and display the content in the best way possible for that device.

## Solution

After reading the Bootstrap docs I found a solution that made creating a responsive site seem easy. Collapsibles are useful when you want to hide and show large amount of content. The .collapse class indicates a collapsible element. This is the content that will be shown or hidden with a click of a button. By added the .collapse class and the css code below I could control when the menu bar would collapse.

```
@media only screen and (max-width: 625px){
  .wrapper{
    grid-template-columns: auto;
  }
}
```

I added this code to manually choose when the max-width would be set because the defaults still made my site look weird on an ipad.

## Results

The result is that I got my site to be a responsive design to run on every platform. Users could now use www.tips4myfirsthouse on their phones as well as on their home computers. This was important so users could add tasks to their custom checklist at the time of looking for a house on their cell phones.

## Conclusion

I learned the hard way that when building an application, if you want my users to have the best possible experience on mobile and desktop devices, designing for mobile first is the way to go. You won’t have to worry about there being mobile feature constraints, or slower loading times when using a mobile device.
