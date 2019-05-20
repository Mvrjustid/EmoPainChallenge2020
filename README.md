<p align="center">
<img width="700" height="210" src="images/Animation.PNG">
</p>

## Challenge Description
The EmoPain Movement Behavior challenge comprises three tasks based on the EmoPain dataset, participant need to complete at least one of tasks:

- **Task 1**: Protective Movement Behavior Detection from MoCap and surface EMG data: The aim of this task is to build binary classification models to continuosly detect events of protective behaviour (e.g. hesitation) during the execution of an exercise (e.g. sit-to-stand). Data collected from healthy subjects without protective behaviour are also provided. Participants may refer to previous papers [Aung et al. 2014](https://dl.acm.org/citation.cfm?id=2686916), [Aung et al. 2016](https://ieeexplore.ieee.org/abstract/document/7173007), [Wang et al. 2019a](https://arxiv.org/abs/1902.08990), [Wang et al. 2019b](https://arxiv.org/abs/1904.10824). The training and validation set comprise continuous movement data plus sEMG data with **continuous binary** groudtruth labels (per timestep) of selected subjects. The testing set comprises data windows from another pool of participants organized as a set of windows of 3s length and 75% overlapping ratio. The evaluation performance will be computed for such windos segments.

- **Task 2**: Pain-level Recognition from Mocap and surface EMG data: The aim of this taks  is to predict the level of pain perceived by person within a rehabilation exercise on the bases of movement and surface EMG data. Three levels of pain are considered: No Pain, Low-level Pain, High-level Pain. Participants may refer to previous papers [Olugbade et al. 2014](https://dl.acm.org/citation.cfm?id=2663261), [Olugbade et al. 2015](https://ieeexplore.ieee.org/abstract/document/7344578), [Olugbade et al. 2018](https://ieeexplore.ieee.org/abstract/document/8269804), [Olugbade et al. 2019](https://dl.acm.org/citation.cfm?id=3299095). The training and validation set comprise movement instances (complete movement segments) of each selected subjects, while groudtruth of 3 categories is providede per instance. The testing set comprises N movement instances of the rest subjects, results reproted from you should be N predicted labels.

- **Task 3**: Pain-level Recognition from facial expression features: The aim of this task is to continuosly predict a person's pain-level from their facial expression. Participants may refer to previous papers [Aung et al. 2016](https://ieeexplore.ieee.org/abstract/document/7173007). The training and validation set comprise continuos instances of facial features extracted from videos of participants (healthy and people suffering from chronic pain) during physical activity.



## Dataset

The EmoPain dataset contains facial expressions, full-body MoCap data and surface EMG data collected from 4 places on the back, captured from 12 healthy subjects and 18 patients with chronic lower back pain while doing physical exercise. 
<br>
<br>
For the facial expression, continuous labelling of pain levels is provided. For the movement behavior data, continuous labelling of protective movement behavior is provided per timestep, while the label of pain-level is provided per exercise instance.
<br>
Due to GDPR regulations, the specific data we included are low-level mathematic features of the original data: 
- **Angles** (calculated from each three relevant anatomical points) and **Energies** (the respective angular velocities) for the description of movement. See the diagram took from [Wang et al. 2019b](https://arxiv.org/abs/1904.10824):

<p align="center">
<img width="400" height="320" src="images/Angle.PNG">
</p>

- **Upper envelope of the surface EMG data** for the description of muscle activity. See the diagrams took from [Aung et al. 2016](https://ieeexplore.ieee.org/abstract/document/7173007), [Wang et al. 2019a](https://arxiv.org/abs/1902.08990):

<p align="center">
<img width="160" height="240" src="images/sEMGcapture.PNG">
<img width="333" height="252" src="images/sEMG.PNG">
</p>
<p align="center">
As a result, the data matrix provided will be like:
</p>
<p align="center">
<img width="776" height="192" src="images/data.PNG">
</p>

- **Facial geometric feature plus deep feature** for the pain recognition from facial expression. Details coming soon. 

The dataset is divided randomly into 
- Training Set (10 patients, 6 healthy subjects)
- Validation Set (4 patients, 3 healhy subjects)
- Testing Set (4 patients, 3 healthy subjects)

## Participate
To participate in the EmoPain movement behavior challenge, please download, fill and sign the form (link is coming soon).
<br>
Then return the form to 
<br>
emopain19@gmail.com
<br>

After the release of testing data, each team has 5 chances to upload the required results.

The performance rank will only be put online before the workshop day.

## Metric
For task 1 and 2, we use the mean F1 score as the metric:

<p align="center">
<img width="272" height="64" src="images/meanf1.PNG">
</p>

where the pre and recall is the precision and recall ratio of class c (c=2, protective and non-protective).

For task 3, more information to come soon.

## Paper Submission
Paper will be submitted through EasyChair(Link is coming soon).
<br>
We are expecting at least 20 submissions and we plan a 50% acceptance rate. 
<br>
We have received many requests for access to the EmoPain dataset and this challenge is an opportunity to open it. 
<br>
Paper length will be up to 7 pages (6 pages + 1 page for references). 
The reviewing process will be double blind.

## Important Dates

- Training and Validation Data Available: 24th of May, 2019
- Testing Data Available: 31th of May, 2019 
- Results Uploading Deadline: 9th of June, 2019
- Paper Submission Deadline: 18th of June 2019
- Notification: 8th of July 2019 
- Camera Ready due: 12th of July, 2019 
- Workshop Date: 3rd of September, 2019

## Keynote Speakers

#### [Professor Rebecca Slater, Oxford University, UK (tentative)](https://www.paediatrics.ox.ac.uk/team/rebeccah-slater)
#### [Professor Chris Eccleston, University of Bath, UK (tentative)](https://researchportal.bath.ac.uk/en/persons/chris-eccleston)

We also aim to have a multidisciplinary panel (in line with the inclusion theme of ACII 2019) on the requirements and challenges from 
real world applications for the above-discussed technology.
<br>
We hope that the discussion will trigger interest that leads to new approaches for developing automatic recognition systems. 
<br>
The panel will be led by a member of the organizing committee (Dr Amanda Williams, clinical psychologist and academic expert in pain) and include 2 keynote speakers (see above), a senior physiotherapist (Mr Diarmuid Denneny, Pain Management Centre, UCLH NHS Foundation Trust, UK) and an HCI researcher (Dr Aneesha Singh, UCL, with long-term research experience with pain patients).
