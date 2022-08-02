---
layout: default
title: (Shamelessly) Pirating my own games
---
# (Shamelessly) Pirating my own games

***

Ten years ago I was making my first games. They were pretty terrible but I didn't know any better. I published a couple on kongregate and moved on.

Now I'm trying to make those games playable again. They were built in Flash, which is basically impossible to use these days. Fortunately, I still have the original project files. After some researching, I found that [newgrounds has native support for Flash via Ruffle](https://www.newgrounds.com/bbs/topic/1448692) - a flash emulator that runs in the browser!

Excited, I loaded up my game, clicked play, and held my breath as the load bar filled up. A second later, I was greeted with this fullscreen prompt:

![Full-screen sitelock. Got 'em](/assets/images/pirate/sitelock1.png){: width="400px" style="display: block;margin-left: auto;margin-right: auto"}

Full-screen sitelock. Got 'em
{: class="caption"}

Apparently, I was very concerned that someone was going to come along and steal my very first games! I added a sitelock so that they could only be played on kongregate. My upload to newgrounds was blocked!

While I'm sure my younger self got a good chuckle out of the wording, I wasn't about to let him keep me from reviving my old games.

**Attempt 1:** Maybe I could just add `?kongregate.com` into the URL and fool the sitelock check. No dice - the sitelock was only searching for the string in the domain itself.

**Attempt 2:** open the .swf file in a hex editor. Search for `kongregate` so that I could edit the sitelock domain. Unfortunately, this was pretty naive - .swf files are compiled.

**Attempt 3:** While doing some research I stumbled across [JPEXS](https://github.com/jindrapetrik/jpexs-decompiler), a .swf decompiler. This was exactly what I needed - the project loaded in without any issues! I could now go to the sitelock code and bypass it.

![JPEXS editor with the sitelock disabled](/assets/images/pirate/jpexs.png){: width="600px" style="display: block;margin-left: auto;margin-right: auto"}

JPEXS editor with the sitelock disabled
{: class="caption"}

With the sitelock disabled it was time to try again. I uploaded the modified .swf, sat through some unnecessarily long logo screens, and made it into the main menu! I loaded up a level and started blasting enemies.

It was wonderful to experience this game again. It was like opening a time capsule that's been sealed for ten years.

![Fly Guy takes to the skies again!](/assets/images/pirate/flyguy1.png){: style="display: block;margin-left: auto;margin-right: auto"}

Fly Guy takes to the skies again!
{: class="caption"}

At the same time, it was also a stark reminder of how little I knew about making games back then. I can't help but laugh at how incomplete this game was and that I prioritized adding DRM over polishing gameplay.

I'm confident that the only person who's tried to pirate this game, is me.

***

I was able to get all of my Flash games playable again! Want to give them a shot?

{% include gameAndDesc.html urlNum=1917852 image="flyguy" name="Fly Guy" desc="Vertical flight action. My first attempt at an original game" %}
{% include gameAndDesc.html urlNum=1918940 image="planet" name="Unfinished Gravity Planet Sandbox" desc="Gravity-based sandbox. My first published game. Forever in Early Access" %}
{% include gameAndDesc.html urlNum=1917865 image="4way" name="4-Way" desc="Single player pong with four paddles. My first finished game" %}
{% include gameAndDesc.html urlNum=1918943 image="accelerator" name="Accelerator" desc="Physics puzzle prototype. Place accelerator fields to get all the balls to the exit" %}
{% include gameAndDesc.html urlNum=1918949 image="lazer" name="Lazer Mazer" desc="Physics puzzle prototype. Shoot projectiles through a maze to get them to the end" %}
{% include gameAndDesc.html urlNum=1918951 image="dualstick" name="Dual Stick" desc="Action game prototype. Dual-stick based movement while shooting at enemies" %}

