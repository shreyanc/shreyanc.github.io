---
layout: cv
title: Curriculum Vitae
sections:
  - title: Experience
  - title: Education
  - title: Skills
links: >
  <a href="https://www.linkedin.com/in/shreyan-chowdhury/" target="_blank"><i class="fab fa-linkedin"></i> LinkedIn</a> |
  <a href="https://scholar.google.com.au/citations?user=WGjp-vYAAAAJ&hl=en" target="_blank"><i class="ai ai-google-scholar"></i> Google Scholar</a> |
  <a href="https://github.com/shreyanc" target="_blank"><i class="fab fa-github"></i> GitHub</a>
highlights: 
  - title: Latest paper
    description: "DExter: Learning and controlling performance expression with diffusion models"
    image: assets/img/cv_imgs/dexter.png
    link: https://arxiv.org/pdf/2406.14850
    link_title: PDF
    link2: https://river-blackberry-7de.notion.site/DExter-Learning-and-Controlling-Performance-Expression-through-Diffusion-models-5ee49ab5db68402b883f2f288022661a
    link_title2: Demo
    link3: https://github.com/anusfoil/DExter
    link_title3: Code

  - title: Real-time musical emotion tracking
    description: Predicting Jacob Collier's musical emotions through his piano playing
    image: assets/img/cv_imgs/jc2.png
    link: https://www.youtube.com/watch?v=1Y8wDZfuaKU
    link_title: YouTube Video

  - title: My PhD Thesis
    description: Modelling Emotional Expression in Music Using Interpretable and Transferable Perceptual Features
    image: assets/img/cv_imgs/phd1.png
    link: https://epub.jku.at/obvulihs/content/titleinfo/8165733/full.pdf
    link_title: PDF

  - title: Magazine Article
    description: My research covered in IIT Madras Shaastra Magazine
    image: assets/img/cv_imgs/shaastra.png
    link: https://shaastramag.iitm.ac.in/lead-story/high-notes
    link_title: Article

  - title: My most-cited paper
    description: "Towards Explainable Music Emotion Recognition: The Route via Mid-level Features"
    image: assets/img/cv_imgs/midlevel_expl.png
    link: https://arxiv.org/pdf/1907.03572
    link_title: PDF

  - title: Patent on audio-based predictive maintenance
    description: "Monitoring industrial equipment using audio"
    image: assets/img/cv_imgs/hwellh.png
    link: https://patentimages.storage.googleapis.com/f8/31/56/ac87627fd984e8/US11348598.pdf
    link_title: Patent PDF

  # - title: Achievement C
  #   description: Details of Achievement C
---

<style>
  h3 {
    margin-bottom: 0.1em;  /* Reduce space below h3 */
  }
  h3 + p {
    margin-top: -0.3em;  /* Reduce space above the paragraph following h3 */
  }

  p + ul {
    margin-top: -0.8em;  /* Reduce space between paragraph and list */
  }
</style>

## Experience
### Co-Founder and Chief Science Officer
{% include company_date.html company="SongForm, Inc." location="Remote" date="Nov 2023 - Present" %}
- Building tools for human-AI music co-creation.
- Trained voice conversion and music accompaniment generation models.

### Machine Learning Consultant (Contract)
{% include company_date.html company="Bogren Digital" location="Remote" date="May 2023 - Nov 2023" %}
- Proposed architectures for modelling vintage audio effects hardware.
- Improved existing RNN and LSTM models for guitar amp modelling.

### Postdoctoral Researcher
{% include company_date.html company="Johannes Kepler University Linz" location="Linz, Austria" date="Jan 2023 - Dec 2023" %}
- Supervisor: [Prof. Gerhard Widmer](https://www.jku.at/en/institute-of-computational-perception/about-us/people/gerhard-widmer/){:target="_blank"}
- Developed an expressivity-aware music retrieval system.
- Proposed a diffusion model for steerable piano performance generation.

### Scientific Staff (PhD researcher)
{% include company_date.html company="Johannes Kepler University Linz" location="Linz, Austria" date="May 2018 - Dec 2022" %}
- Advisor: [Prof. Gerhard Widmer](https://www.jku.at/en/institute-of-computational-perception/about-us/people/gerhard-widmer/){:target="_blank"}
- Proposed novel techniques for explainable music emotion recognition using mid-level feature learning and domain adaptation.
- Published 9 papers, delivered 2 invited talks at international venues.

### Product Design Engineer
{% include company_date.html company="Honeywell Technology Solutions" location="Bangalore, India" date="July 2015 - May 2018" %}
- Led developemnt of an audio-based condition monitoring system, resulting in a patent and 3 internal awards.
- Patent: Monitoring Industrial Equipment using Audio [[Link]](https://patents.google.com/patent/US10475468B1/en).
- Developed audio anomaly detection models for edge devices.
- Implemented fuzzy control algorithms for Honeywell embedded devices.

<hr>

## Education

### Ph.D. in Computer Science
{% include company_date.html company="Johannes Kepler University Linz" location="Linz, Austria" date="May 2018 - Dec 2022" %}
- Advisor: [Prof. Gerhard Widmer](https://www.jku.at/en/institute-of-computational-perception/about-us/people/gerhard-widmer/){:target="_blank"}
- Thesis: Modelling Emotional Expression in Music Using Interpretable and Transferable Perceptual Features [[pdf]](https://epub.jku.at/obvulihs/content/titleinfo/8165733/full.pdf){:target="_blank"}

### M.Tech. + B.Tech. (Dual Degree) in Electrical Engineering
{% include company_date.html company="Indian Institute of Technology Kanpur (IIT-Kanpur)" location="Kanpur, India" date="Jul 2010 - Jul 2015" %}
- Specialization: Signal Processing
- Advisor: [Prof. Rajesh Hegde](https://rajeshmhegde.com/){:target="_blank"}
- Thesis:  Musical Tempo Estimation Using Sub-band Synchrony [[pdf]](assets/pdf/mtech_thesis.pdf){:target="_blank"}

<hr>

## Publications

{% capture my_text %}
1. DExter: Learning and controlling performance expression with diffusion models. [[HTML]](https://www.mdpi.com/2076-3417/14/15/6543){:target="_blank"} [[PDF]](https://arxiv.org/pdf/2406.14850){:target="_blank"} [[Demo]](https://river-blackberry-7de.notion.site/DExter-Learning-and-Controlling-Performance-Expression-through-Diffusion-models-5ee49ab5db68402b883f2f288022661a){:target="_blank"} [[Code]](https://github.com/anusfoil/DExter){:target="_blank"} <br> H Zhang, <u>S Chowdhury</u>, CE Cancino-Chacón, J Liang, S Dixon, G Widmer (2024). <br> MDPI Applied Sciences, 14(15), 6543. 

2. Expressivity-aware Music Performance Retrieval using Mid-level Perceptual Features and Emotion Word Embeddings. [[PDF]](https://dl.acm.org/doi/pdf/10.1145/3632754.3632761) <br> <u>S Chowdhury</u>, G Widmer (2023). <br> Proceedings of the 15th Annual Meeting of the Forum for Information, Goa, India.

3. Are we describing the same sound? An analysis of word embedding spaces of expressive piano performance. [[PDF]](https://dl.acm.org/doi/pdf/10.1145/3632754.3632759){:target="_blank"} <br> SD Peter, <u>S Chowdhury</u>, CE Cancino-Chacón, G Widmer (2023)<br> Proceedings of the 15th Annual Meeting of the Forum for Information, Goa, India.

4. Decoding and Visualising Intended Emotion in an Expressive Piano Performance. [[PDF]](https://arxiv.org/pdf/2303.01875){:target="_blank"} [[Demo Video]](https://www.youtube.com/watch?v=1Y8wDZfuaKU){:target="_blank"} <br> <u>S Chowdhury</u>, G Widmer (2022)<br> ISMIR. Late-Breaking Demo Session of the 23rd Int. Society for Music Information Retrieval Conf., Bengaluru, India

5. Modelling emotional expression in music using interpretable and transferable perceptual features. [[PDF]](https://epub.jku.at/obvulihs/content/titleinfo/8165733/full.pdf){:target="_blank"} <br> <u>S Chowdhury</u> (2022)<br> Ph. D. Thesis.

7. On perceived emotion in expressive piano performance: Further experimental evidence for the relevance of mid-level perceptual features.<br> <u>S Chowdhury</u>, G Widmer<br> arXiv preprint arXiv:2107.13231.

8. Tracing Back Music Emotion Predictions to Sound Sources and Intuitive Perceptual Qualities.<br> <u>S Chowdhury</u>, V Praher, G Widmer<br> Proceedings of the 18th Sound and Music Computing Conference, 246-252.

9. Towards explaining expressive qualities in piano recordings: Transfer of explanatory features via acoustic domain adaptation.<br> <u>S Chowdhury</u>, G Widmer<br> ICASSP 2021-2021 IEEE International Conference on Acoustics, Speech and.

10. Receptive-field regularized CNNs for music classification and tagging.<br> K Koutini, H Eghbal-Zadeh, V Haunschmid, P Primus, <u>S Chowdhury</u>, ...<br> arXiv preprint arXiv:2007.13503.

11. On the Characterization of Expressive Performance in Classical Music: First Results of the Con Espressione Game.<br> C Cancino-Chacón, S Peter, <u>S Chowdhury</u>, A Aljanaki, G Widmer<br> Proceedings of the 21st International Society for Music Information.

12. Monitoring industrial equipment using audio.<br> R Yelchuru, <u>S Chowdhury</u>, P Sampath<br> US Patent 10,475,468.

13. Emotion and theme recognition in music with frequency-aware RF-regularized CNNs.<br> K Koutini, <u>S Chowdhury</u>, V Haunschmid, H Eghbal-Zadeh, G Widmer<br> arXiv preprint arXiv:1911.05833.

14. Two-level Explanations in Music Emotion Recognition.<br> V Haunschmid, <u>S Chowdhury</u>, G Widmer<br> International Conference on Machine Learning (ICML), Machine Learning for.

15. Towards Explainable Music Emotion Recognition: The Route via Mid-level Features.<br> <u>S Chowdhury</u>, A Vall, V Haunschmid, G Widmer<br> Proceedings of the 20th International Society for Music Information.

16. Music tempo estimation using sub-band synchrony.<br> <u>S Chowdhury</u>, T Guha, RM Hegde<br> Proceedings of Interspeech 2017, 3093-3096.

17. Musical Tempo Estimation from Audio using Sub-Band Synchrony.<br> <u>S Chowdhury</u><br> INDIAN INSTITUTE OF TECHNOLOGY, KANPUR.
{% endcapture %}

{% include collapsible_box.html content=my_text %}


## Certifications
- Machine Learning in Production [[Coursera]](https://coursera.org/verify/X6R5D6VCZQMN){:target="_blank"}
- Improving Deep Neural Networks: Hyperparameter Tuning, Regularization and Optimization [[Coursera]](https://coursera.org/verify/Z5UFPV5HVAS8){:target="_blank"}
- Digital Sound Design [[Coursera]](https://shreyanc.github.io/assets/pdf/Coursera_Certificate_v1-970242443205.pdf){:target="_blank"}


## Achievements

- Work recognized in Shaastra Magazine [[Article]](https://shaastramag.iitm.ac.in/lead-story/high-notes)
- 1st rank, MediaEval Mood Recognition Challenge 
- Tech & Innovation Award, Honeywell 
- Outstanding Achiever Award, Honeywell
- 99.86 percentile in IIT-JEE

## Service
   - **Peer-reviewer**:
     - ICNMC conference (2023)
     - ISMIR conference (2020-2024)
   - **Mentor**:
     - WiMIR (Women in MIR) (2022-2023)
     - Institute summer internship (2022)
   - **Course Teaching Assistant**:
     - Artificial Intelligence (2023)
     - Electrical Engineering Lab (2014-2015)

## Languages

- English (Fluent)
- German (Intermediate: [[B1-level]](assets/pdf/Zeugnis.PDF){:target="_blank"})
- Hindi (Native)
- Bengali (Native)

<!-- [Download PDF Version](assets/pdf/Resume_Shreyan_Chowdhury.pdf) -->

