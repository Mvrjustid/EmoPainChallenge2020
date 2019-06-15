<p align="center">
<img width="700" height="210" src="images/Animation.PNG">
</p>

## Challenge Description
The EmoPain Challenge 2019 comprises three tasks. Participants should complete at least one of them. The tasks are based on the EmoPain dataset and are as follows:

- **Movement Behaviour Classification Task**: The aim of this task is to build a binary classification model to continuously detect events of protective behaviour (e.g. hesitation) in participants with chronic lower back pain (CLBP) during exercise performance (e.g. sit-to-stand), based on body movement and muscle activity. We provide training, validation, and test data, which comprise joint angles and energies as well as surface electromyography (sEMG) data from both participants with CLBP and healthy control participants. The data comes with **continuous binary** labels (i.e. one label per timestep). Participants should see below for details about these data, and how to access the data for this task. A README document will be attached to the data to provide more detailed information.  

- **Pain Recognition from Movement Task**: The aim of this task is to build a classification model to differentiate between a participant with CLBP and a healthy control participant as well as differentiate between two levels of self-reported pain for participants with CLBP (in essence, classification of three levels of pain: Healthy, Low-level Pain, High-level Pain), based on body movement and muscle activity during exercise performance. We provide training, validation, and test data, which comprise joint angles and energies as well as sEMG data from both participants with CLBP and healthy control participants. The data comes with three class labels per instance. Participants should see below for details about these data, and how to access the data for this task. A README document will be attached to the data to provide more detailed information.

- **Pain Face Recognition Task**: The aim of this task is to build a detection model to differentiate between a participant with CLBP and a healthy control participant as well as continuously recognise the levels of observer-rated pain of participants with CLBP, based on facial expression during exercise performance. We provide training, validation, and test data, which comprise features extracted from face video data from both participants with CLBP and healthy control participants. Participants should see below for details about these data, and how to access the data for this task. A README document will be attached to the data to provide more detailed information.



## Dataset

- **Joint Angles** and **Joint Energies** (calculated from the joint angles). See diagram below, taken from [Wang et al. 2019b](https://arxiv.org/abs/1904.10824):

<p align="center">
<img width="400" height="320" src="images/Angle.PNG">
</p>

- **sEMG data**. The data given is the upper envelope of the rectified sEMG sensor data. See diagram on left below for the placement of the sensors, taken from [Aung et al. 2016](https://ieeexplore.ieee.org/abstract/document/7173007)

<p align="center">
<img width="160" height="240" src="images/sEMGcapture.PNG">
<img width="333" height="252" src="images/sEMG.PNG">
</p>


- **Facial geometric feature plus deep feature** for the pain recognition from facial expression. Details coming soon. 

## Dataset Partition
The dataset is divided randomly into 
- Training Set (10 patients, 6 healthy subjects)
- Validation Set (4 patients, 3 healhy subjects)
- Testing Set (4 patients, 3 healthy subjects)

## Participate
To participate in the EmoPain Challenge 2019, please download, fill, and sign the EULA (link coming soon). The form should then be sent to **emopain19@gmail.com**.
<br>

When we receive the form, the link to the training and validation sets will be emailed to the sender. At a later date, the link to the test set will also be forwarded.
<br>
The test set results should be sent by each participating team to the email address above. Each team can submit up to 5 different results. 
<br>
The test results performance ranking will be based on the metric described below. The ranking over all will be displayed on this website, before the workshop day.

## Metric
For the Movement Behaviour Classification and the Pain Recognition from Movement tasks, we will use the mean F1 score as the performance metric:

<p align="center">
<img width="272" height="64" src="images/meanf1.PNG">
</p>

where _pre_ and _recall_ are the precision and recall ratios respectively of class _c_.

For task 3, more information to come soon.

## Paper Submission
Papers should be up to 7 pages (6 pages + 1 page for references) and submitted through EasyChair (link coming soon). Please see below for dates. The reviewing process will be double blind.
<br>
We are expecting at least 20 submissions and we plan a 50% acceptance rate. 
<br>

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
