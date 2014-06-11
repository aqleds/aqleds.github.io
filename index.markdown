---
layout: post
---


## Introduction


Finally, we have decided to go open, after lots of work and research, 
AqLeds is ready, and it's free (as in freedom). We're publishing it under 
the GPL license.

* The [mainboard hardware][hardware_main] and the 
  [modular led lamps hardware][hardware_lamp], built on [kicad-pcb][kicad]
* The [firmware][firmware], written in C
* The [PC software][pc], written in Qt C++, to setup your AqLeds.


[kicad]:         http://www.kicad-pcb.org
[hardware_main]: http://github.com/aqleds/hardware_mainboard
[hardware_lamp]: http://github.com/aqleds/hardware_lamps
[firmware]:      http://github.com/aqleds/firmware
[pc]:            http://github.com/aqleds/aqleds


## Video
Accelerated 'lighting' playback of a 12h cycle (night, sunrise, day, sunset, night...).

<iframe src="//player.vimeo.com/video/70742978" width="800" height="469" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe> 

## Getting started

* Get a preassembled board

## Development

### Tools
* MPLAB.X + XC16 compiler
* Qt designer on the PC side for the configuration client. 

## DIY

* Assemble a board
* Write the PIC with the bootloader
* Write the firmware using the bootloader and the client software
* Test it
* Start using it.



<div class="home">
  <br/>
  <h1>Posts</h1>

  <ul class="posts">
    {% for post in site.posts %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>
