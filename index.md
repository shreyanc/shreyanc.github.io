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
## Publications

[On Perceived Emotion in Expressive Piano Performance: Further Experimental Evidence for the Relevance of Mid-level Features](https://arxiv.org/abs/2107.13231)
> **Shreyan Chowdhury**, Gerhard Widmer<br>
> ISMIR 2021, Virtual

[Tracing Back Music Emotion Predictions to Sound Sources and Intuitive Perceptual Qualities](https://arxiv.org/abs/2106.07787)
> **Shreyan Chowdhury**, Verena Praher, Gerhard Widmer<br>
> Sound and Music Computing Conference 2021

[Towards Explaining Expressive Qualities in Piano Recordings: Transfer of Explanatory Features via Acoustic Domain Adaptation](https://arxiv.org/abs/2102.13479)
> **Shreyan Chowdhury**, Gerhard Widmer<br>
> ICASSP 2021, Toronto, Canada


[The Con Espressione Game Dataset (1.0.0)](https://doi.org/10.5281/zenodo.3968828)
> Carlos Cancino-Chacón, Silvan Peter, **Shreyan Chowdhury**, Anna Aljanaki, Gerhard Widmer<br>
> ISMIR 2019, Montreal, Canada

[On the Characterization of Expressive Performance in Classical Music: First Results of the Con Espressione Game](https://arxiv.org/abs/2008.02194)
> Carlos Cancino-Chacón, Silvan Peter, **Shreyan Chowdhury**, Anna Aljanaki, Gerhard Widmer<br>
> ISMIR 2019, Montreal, Canada



[Emotion and Theme Recognition in Music with Frequency-Aware RF-Regularized CNNs](https://www.jku.at/fileadmin/gruppen/173/Research/Emotion_in_Music_with_Frequency-Aware_RF-Regularized_CNNs_Koutini.pdf)
> Khaled Koutini, **Shreyan Chowdhury**, Verena Haunschmid, Hamid Eghbal-zadeh, Gerhard Widmer<br>
> MediaEval Multimedia Benchmark 2019, Sophia Antipolis

[Towards Explainable Music Emotion Recognition: The Route via Mid-level Features](https://arxiv.org/abs/1907.03572) [[demo]](https://shreyanc.github.io/ismir_example.html)
>**Shreyan Chowdhury**, Andreu Vall, Verena Haunschmid, Gerhard Widmer<br>
>ISMIR 2019, Delft, Netherlands

[Two-level Explanations in Music Emotion Recognition](https://arxiv.org/abs/1905.11760) [[demo]](https://shreyanc.github.io/ICML_example.html)
>Verena Haunschmid, **Shreyan Chowdhury**, Gerhard Widmer<br>
>ICML 2019, Machine Learning for Music Discovery Workshop



[Music Tempo Estimation Using Sub-Band Synchrony](https://www.isca-speech.org/archive/Interspeech_2017/pdfs/1000.PDF) [[poster]](http://tanayag.com/Pub_files/chowdhury_ISposter.pdf)
>**Shreyan Chowdhury**, Tanaya Guha, Rajesh M Hegde<br>
>INTERSPEECH, 3093-3096
