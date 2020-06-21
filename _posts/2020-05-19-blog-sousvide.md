---
title: 'Sous Vide at home'
date: 2020-05-19
permalink: /posts/2020/05/sousvide/
excerpt: "My recent attempt to low-temperature cooking with a DIY system   <br/><img src='/images/sous-vide-2.JPG'>"
tags:
  - quarantine
  - cooking
---

Hello! Wish you are doing as best as you can during the COVID-19 pandemic. Here I am sharing my recent attempt to low-temperature cooking.

Like everyone else, I am spending a lot of time staying at home. My roommate and I take turns in cooking and we have meals together. Inspired by my father, I became interested to experiment on low-temperature cooking, aka Sous Vide, at home. I found that Sous Vide is quite popular because it is said to create a uniform "readiness" of the item. While for stove-top cooking, I sometimes see the item is raw inside when the outside is well done. The working principle for Sous Vide is simple - immerse the item (sealed in a vacuum bag) in a water bath that maintains a constant but low temperature ~ 120-140ºF (50-60ºC), for 1-3 hours typically.  

However, commercial Sous Vide units are pretty expensive (~$100) for an amateur cook like me. Given that a constant temperature water bath is the only thing needed, I decided to try it in a simple way.

So here is how I implement it, with a pot plugged into a temperature controller that turns the pot on and off based on the feedback from a thermocouple.

Hardware
------

- a pot that could start heating once it is plugged in
- a temperature controller

For the pot, some advanced pots with smart functionalities may not be ideal, especially if they need us to push buttons before they turn on the heater. I tried out the pots we have in the kitchen and found one that works.

For the temperature controller, they are easily available online (~$30 for my WILLHI WH1436A). This module is not even PID controlled, but works well for my cooking purpose. For folks that would like to dive more into it, programming an Arduino board, among others, might worth a try.

![photo1](/images/sous-vide-2.JPG)

Procedure
-----
1. Let the item to be cooked return to room temperature. Seal it in a bag and remove air inside - an easy way is to immerse the bag halfway in the water bath, so that the majority of air would be pushed out of the bag by hydraulic pressure.

2. Plug in the temperature controller to an outlet, and plug in the pot to the controller. Fill the pot with water. Immerse the item in the water bath. Put the end of the thermocouple (its sensing part) in the water bath near the item, for more accurate measurement.

3. Set parameters on the temperature controller and start cooking. For WH1436A, I was able to set an ON temperature, below which the power will be on, and an OFF temperature, above which the power will be off. The temperature settings are based on the item (whether it is chicken or beef, steak or roast, etc) and the doneness of choice. I referred to [this website](https://www.chefsteps.com/activities/sous-vide-time-and-temperature-guide) for rough ideas. I followed their suggestions on the cooking duration, too.

4. Take the item out when time is up. Shut off all appliances safely.

5. Sear the item on the stove, and season it with salt, pepper and/or herbs that you like.

6. Enjoy!



