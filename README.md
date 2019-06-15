<p align="center">
<img width="700" height="210" src="images/Animation.PNG">
</p>

## Challenge Description
The EmoPain challenge comprises three tasks. Participants should complete at least one of them. The tasks are based on the EmoPain dataset and are as follows:

- **Movement Behaviour Classification Task**: The aim of this task is to build a binary classification model to continuously detect events of protective behaviour (e.g. hesitation) in participants with chronic lower back pain (CLBP) during exercise performance (e.g. sit-to-stand), based on body movement and muscle activity. We provide training, validation, and test data, which comprise joint angles and energies as well as surface electromyography (sEMG) data from both participants with CLBP and healthy control participants. The data comes with **continuous binary** labels (i.e. one label per timestep). Participants should see below for details about these data, and how to access the data for this task. A README document will be attached to the data to provide more detailed information.  

- **Pain Recognition from Movement Task**: The aim of this task is to build a classification model to differentiate between a participant with CLBP and a healthy control participant as well as differentiate between two levels of self-reported pain for participants with CLBP (in essence, classification of three levels of pain: Healthy, Low-level Pain, High-level Pain), based on body movement and muscle activity during exercise performance. We provide training, validation, and test data, which comprise joint angles and energies as well as sEMG data from both participants with CLBP and healthy control participants. The data comes with three class labels per instance. Participants should see below for details about these data, and how to access the data for this task. A README document will be attached to the data to provide more detailed information.

- **Pain Face Recognition Task**: The aim of this task is to build a detection model to differentiate between a participant with CLBP and a healthy control participant as well as continuously recognise the levels of observer-rated pain of participants with CLBP, based on facial expression during exercise performance. We provide training, validation, and test data, which comprise features extracted from face video data from both participants with CLBP and healthy control participants. Participants should see below for details about these data, and how to access the data for this task. A README document will be attached to the data to provide more detailed information.



## Dataset

- **Joint Angles** (calculated from each three relevant anatomical points) and **Joint Energies** (the respective angular velocities) for the description of movement. See the diagram took from [Wang et al. 2019b](https://arxiv.org/abs/1904.10824):

<p align="center">
<img width="400" height="320" src="images/Angle.PNG">
</p>

- **Upper envelope of the sEMG data** for the description of muscle activity. See the diagrams took from [Aung et al. 2016](https://ieeexplore.ieee.org/abstract/document/7173007), [Wang et al. 2019a](https://arxiv.org/abs/1902.08990):

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
**emopain19@gmail.com** 
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

- Training and Validation Data Available: 14th of June, 2019
- Testing Data Available: 19th of June, 2019 
- Results Uploading Deadline: 24th of June, 2019
- Paper Submission Deadline: 25th of June 2019
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
