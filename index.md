---
title: Home
---

# Foundational Model for Visual Perception (FM4VP) Challenge

in accordance with [VPLOW workshop](https://vplow.github.io/vplow_3rd.html) at CVPR 2023, Vancouver, Canada.

{% include figure.html img="car-images.png" alt="intro image here" caption="SOFAR (SOCAR: Socially-Obtained CAR image dataset" width="99%" %}


---

<!-- <div class="toc" markdown="1"> -->
## Introduction

This year, in accordance with Visual Perception via Learning in an Open World (VPLOW) workshop, we firstly organize Foundational Model for Visual Perception (FM4VP) challenge in CVPR 2023. This year's FM4VP challenge proposes a zero-shot/few-shot image classification problem leveraging FMs (i.e., CLIP, CoCa), to deal with novel samples in the real world. From an industry perspective, when novel samples occur in the business, we may retrieve and annotate every novel sample to re-train the model. However, it becomes too expensive if we perform this procedure whenever novel samples occur. To this end, utilizing the zero-shot/few-shot classification ability of recently-proposed foundational models can be a reasonable & presumable solution. Therefore, we hereby aim to empower candidate workshop participants to contemplate this challenge and let the students, researchers, and Machine Learning community access the industry-level dataset retrieved in the real world. 

---

<!-- </div> -->


<!-- <div class="toc" markdown="1"> -->
## Orgainizers

The FM4VP Challenge 2023 is hosted by SOCAR. SOCAR is the largest car-sharing platform in Repbulic of Korea, providing a seamless mobility experience from car, public transportations, parking lots, electric bike, and even autonomous vehicles. The organizers are applied research scientists at SOCAR, and currently researching/developing on AI products for the business impact in the real world.

<img src="images/organizers-3.png">

---
<!-- </div> -->

<!-- <div class="toc" markdown="1"> -->
## Problem Statement: Zero/Few-shot Image Classification with Foundational Models

In this year's FM4VP challenge, we propose a business problem called car state classification in the open world. A car state classification aims to recognize a car's various statuses (i.e., exterior damage, dirt, wash, etc.) that occur in the real world, especially in SOCAR, the largest car-sharing platform in the Republic of Korea. The SOCAR requires its users to take pictures of cars before they drive, to monitor the car's status. Based on these images, SOCAR establishes an image classifier that identifies the car's various statuses and performs follow-up business actions for efficient business operation (i.e., washing the car if 'exterior dirt' is detected, sending the car if harsh damage is detected). The most challenging part of managing this classifier is dealing with novel samples occurring in the real world. For example, how can we identify novel patterns of dirty cars? How can we recognize novel damage patterns such as harsh car breakage or accident? To resolve these challenges, leveraging FM's effectiveness, we propose the real-world car image dataset and empower the participants to solve this problem. 
<!-- </div> -->
---

<!-- <div class="toc" markdown="1"> -->
## Dataset

In this challenge, we are releasing SOCAR (Socially-Obtained CAR) dataset, which includes ten-thousand car images retrieved from the real world car-sharing operation. For a detailed description of the SOCAR dataset, please refer to the paper [SOCAR: Socially-Obtained CAR Dataset for Image Recognition in the Wild]('https://openaccess.thecvf.com/content/WACV2023W/DNOW/papers/Seo_SOCAR_Socially-Obtained_CAR_Dataset_for_Image_Recognition_in_the_Wild_WACVW_2023_paper.pdf')

The **Training Set** includes 13 classes, each representing car's status that the car-sharing platform can easily understand.

* Exterior Normal
* Exterior Damage
* Bubble Wash
* Car in a Washing machine
* Dashboard
* Cupholder
* Glovebox
* Washer Fluid
* Front Seat
* Read Seat
* Trunk
* Clean Sheet
* Tire

In a **Support Set** (which can be used under the few-shot learning setting), we provide 6 additional classes which cannot be easily expected in the real world. However, it becomes more challenging in the open-world setting as the pattern of these classes is diverse and cannot be expected a priori.

* Exterior Dirt
* Dirty Cupholder
* Dirty Sheet
* Dirty Seat
* Car on a rainy day
* Car on a snowy day

In the **Test Set**, we provide a total of 19 classes of car status, which concatenates classes at both the Training and Support set.

<!-- </div> -->

---
<!-- <div class="toc" markdown="1"> -->
## Evaluation
In this FM4VP Challenge 2023, we will measure **Macro F1-Score** as an evaluation metric. Under the given Test set, participants submit prediction results at each corresponing test samples. The submission format (.csv) is included in the dataset. After the participants submit their file to the submission site, it will be uploaded to the leaderboard.

<!-- </div> -->
---
<!-- <div class="toc" markdown="1"> -->
## Important Dates:

* May 10, 2023: Release of Training Set and Validation Set
* May 15, 2023: Leaderboard Open
* June 15, 2023: Challenge Deadline
* June 18, 2023: VPLOW workshop

Please Note that every deadlines are 23:59 in AoE timezone except for the VPLOW workshop date.

<!-- </div> -->

---
<!-- <div class="toc" markdown="1"> -->
## Contact:

* Kyung Ho Park (kp@socar.kr)
* Hyunhee Chung (esther@socar.kr)
* Taewon Seo (cillian@socar.kr)
* Sanghuk Lee (leonard@socar.kr)
* Hyeonsoo Kim (lucci@socar.kr)

<!-- </div> -->


Hosted by [SOCAR](https://www.socar.kr/), {{ site.pub_year }}.
 
> built using [Jekyll](https://jekyllrb.com/) and [GitHub Pages](https://pages.github.com/)
>
> images and content: cc-by-sa <a href="https://github.com/{{ site.github_username }}">{{ site.author }}</a> {{ site.pub_year}} (get [source code]({{ site.repo }})).
> Last build date: {{ site.time | date: "%Y-%m-%d" }}.
>
> <a href="http://creativecommons.org/licenses/by-sa/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" alt="Creative Commons License" /></a>
