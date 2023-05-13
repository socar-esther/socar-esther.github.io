---
title: Dataset & Submission
nav: true
---

# Dataset Access
Please read the [Form](https://forms.gle/DMGPiHZhNHYzCxhP8) carefully and fill in the required information if you agree. The dataset download URL will be provided if you complete the form. The structure of the dataset is illustrated below.

```
Train 
L 01_outer_normal
    L train_01_outer_normal_0.png
    ...
L ...

Validation
L 01_outer_normal
    L validation_01_outer_normal_0.png
    ...
L ..

Test
ㄴ 0.png
ㄴ 1.png
ㄴ ...
```



# Submission
Please submit your prediction results on the Test set at this [Submission Form](https://docs.google.com/forms/d/12tlYs3qAAOGSGypC2itHQhbFtAK9PTyjZvFTZndzq9s/viewform?edit_requested=true). If you submit more than one submission in a day (PST), the final submission will be only recorded in the leaderboard. 

You can train your model with the training set, check the trained model's performances with the validation set. When you submit your final results on the test set, fill in the prediction results at the attached submission_format.csv. Please follow the label name below. In the prediction column of the submission_format.csv, the inserted value should be one of the values in the label names provided below. Derivations from the given label names (i.e., 01 / outer_normal / normal / 0 for 01_outer_normal) will not be evaluated.

```
01_outer_normal
02_outer_damage
03_outer_dirt
04_outer_wash
05_inner_wash
06_inner_dashboard
07_inner_cupholder
08_inner_cupholder_dirt
09_inner_glovebox
10_inner_washer_fluid
11_inner_front_seat
12_inner_rear_seat
13_inner_trunk
14_inner_sheet_clean
15_inner_sheet_dirt
16_inner_seat_dirt
17_outer_rainy
18_outer_snowy
19_outer_tire
```