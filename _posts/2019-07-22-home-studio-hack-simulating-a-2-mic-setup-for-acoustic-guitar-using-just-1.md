---
layout: post
published: false
title: 'Home Studio Hack: Simulating a 2-mic setup for acoustic guitar using just 1 '
---
To get more ambience and stereo width when recording, say an acoustic guitar, the common practice is to record with two microphones placed at different angles or locations and panning them left and right. This is super useful when the guitar is used for accompanying a lead vocalist or instrumentalist, as it creates room in the mix for the central voice. 

Some useful techniques for micing acoustic guitars can be found in this video:
<iframe width="560" height="315" src="https://www.youtube.com/embed/vmQfVv_cn84" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

But what do you do if you have just one mic? 

One option, especially if you recording over a click track, is to record the same part twice and pan one to the left and the other to the right. The slight differences between the two performances makes it sound wider when panned this way. But if you are not recording to a click track, or if your part needs to be precise in timing, this might not work, since it can get extremely difficult to match the timings of all your notes in the two performances.

The other option is to use a [stereo enhancement plugin](https://www.image-line.com/support/flstudio_online_manual/html/plugins/Fruity%20Stereo%20Enhancer.htm). What these plugins do is they split the mono audio into two channels - left and right - and introduce a small delay to one of them, thus increasing the stereo width. This is a perfectly viable option, but to me, sometimes, it sounds too dry and artificial, especially when I want the guitar's sound to shine through. 

##The Hack

What I recently did in one of my recordings, was that I made a duplicate track of a single recording (1-mic), panned one of them left and the other right, and passed both of them through [convolution filters](https://en.wikipedia.org/wiki/Convolution_reverb) with two different impulse responses loaded. 

![Annotation 2019-07-22 232234.png]({{site.baseurl}}/img/Annotation 2019-07-22 232234.png)

If you look closely in the screenshot, one of the impulses is bathroom and the other is medium_room. I deliberately chose short impulses because I did not want to introduce too much reverb at this stage.

I turned the dry level all the way down, because I only wanted the modified sound to come out instead of it mixing with the original. You may try playing with the dry:wet ratio for creative purposes. 

FL Studio's Fruity Convolver also gives you option to modify the EQ curves of both the impulse and the output. I cut out the lows and mids in mine to make the sound less "boomy".

![Annotation 2019-07-22 232911.png]({{site.baseurl}}/img/Annotation 2019-07-22 232911.png)

To further enhance the width, I added a very small delay to one of the channels using the delay knob in Fruity Convolver (4 ms). 

![Annotation 2019-07-22 233158.png]({{site.baseurl}}/img/Annotation 2019-07-22 233158.png)

The result sounded quite natural and spacious without having the artificial jarring characteristic of stereo-enhanced signals. 
