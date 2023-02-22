---
layout: default
published: true
is_home_page: true
---
<h1 class="title-center"> Shreyan Chowdhury </h1>

<p style="margin-top: -1em; text-align: center; font-size: small; font-weight: bold"><a href="#" id="show-email">Reveal Email</a></p>
<script>
    var showEmailLink = document.getElementById('show-email');
    var emailID = 'shreyan.chowdhury@jku.at';
    showEmailLink.addEventListener('click', function(event) {
        if (showEmailLink.textContent === 'Reveal Email') {
            showEmailLink.textContent = emailID;
            showEmailLink.href = 'mailto:'+emailID;
            event.preventDefault();
            return false;
            }
        else {
            showEmailLink.textContent = emailID;
            showEmailLink.href = 'mailto:'+emailID;
            }
        });
</script>


I am a post-doctoral researcher in the [Institute of Computational Perception](https://www.jku.at/en/institute-of-computational-perception/about-us/people/shreyan-chowdhury/), a research group under the Department of Computer Science at Johannes Kepler University Linz, Austria. I work in **Artificial Intelligence applied to Audio and Music**. My interests lie in **representation learning** for audio, **explainable** machine learning, **domain adaptation**, audio signal processing, and music information retrieval. 

I received my Ph.D. from Johannes Kepler University Linz, Austria, advised by [Prof. Gerhard Widmer](https://www.jku.at/en/institute-of-computational-perception/about-us/people/gerhard-widmer/). Before that, I was a Product Design Engineer at Honeywell Technology Solutions, Bangalore, India. I hold Masters and Bachelors degrees in Electrical Engineering from Indian Institute of Technology ([IIT-Kanpur](https://en.wikipedia.org/wiki/IIT_Kanpur)), India.

<br>

<!--<ul class="downloads">
  <li><a href="#Publications"><strong>Publications</strong></a></li>
  <li><a href="#"><strong>About Me</strong></a></li>
 </ul>
 
<br><br>-->
---

{% include updates_expandable.html %}

---

{% include publications.html %}