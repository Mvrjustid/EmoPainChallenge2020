<p align="center">
<img width="500" height="150" src="images/Animation1.PNG">
</p>

## Scope
Chronic pain is a major problem facing individuals, families, healthcare providers, and society as a whole. Technology that can assess the behaviour of a person with chronic pain and associated levels of pain and related states could deliver personalised therapies and support in long-term self-management of the condition particularly aiming to improve engagement in valued everyday physical activities. This vision is based on the multidisciplinary approach to chronic pain management advocated by clinicians and grounded in findings in pain research of the importance of addressing pain as a multifaceted experience (with physical, psychological, and social factors and outcomes). The EmoPain challenge provides an opportunity for the FG community to collectively contribute to solving the fundamental problem of automatic detection of pain behaviours and pain levels, based on real data collected from people with chronic pain performing movements that are identical to those that make up daily physical functioning.
<br>

The EmoPain challenge, to be held in conjunction with FG2020 is the first international challenge addressing pain and related behaviour detection. It is based on the EmoPain dataset which contains both face and multimodal movement data from real participants with chronic pain performing physical activity. Previous related benchmark datasets have been aimed at detection from facial cues (The UNBC-McMaster Shoulder Pain Expression Archive Database [Lucey et al. 2011]) or experimental pain (Biovid Heat Pain Database [Walter et al. 2013]) whereas body movement is a critical modality to consider in assessing pain experience. This is also the first time a controlled challenge in pain behaviour is held such that competitors only have access to the training and validation partition, while test partition is held back for performance comparison to ensure a level playing field. Participating teams will be required to send working programs, together with clear documentation of any input and output parameters and the organisers will run thee on the test data. Details of the challenge tasks and guidelines are provided below.
<br>

The organisers will write a baseline paper detailing the Challenge’s objectives, rules and baseline methods for comparison. This will include baseline experimental results on the test partition and would be available on the challenge website from 24th January 2020. To save space, participants are kindly requested to cite the baseline paper instead of reproducing the method descriptions and results contained in the paper.


## Challenge Description
The EmoPain 2020 Challenge consists of three main tasks focussed on pain recognition from facial expressions and body movements, as well as the recognition of pain-related body movements. Participants are expected to complete at least one of them. All tasks are based on the EmoPain dataset and are described as follows:

- **Movement Behaviour Classification Task**: The aim of this task is to build a binary classification model to continuously detect events of protective behaviour (e.g. hesitation) in participants with chronic lower back pain (CLBP) during exercise performance (e.g. sit-to-stand), based on body movement and muscle activity. We provide training, validation, and test data, which comprise joint angles and energies as well as surface electromyography (sEMG) data from both participants with CLBP and healthy control participants. The data comes with **continuous binary** labels (i.e. one label per timestep). Participants should see below for details about these data, and how to access the data for this task. A README document will be attached to the data to provide more detailed information.  

- **Pain Recognition from Movement Task**: The aim of this task is to build a classification model to differentiate between a participant with CLBP and a healthy control participant as well as differentiate between two levels of self-reported pain for participants with CLBP (in essence, classification of three levels of pain: Healthy, Low-level Pain, High-level Pain), based on body movement and muscle activity during exercise performance. We provide training, validation, and test data, which comprise joint angles and energies as well as sEMG data from both participants with CLBP and healthy control participants. The data comes with three class labels per instance. Participants should see below for details about these data, and how to access the data for this task. A README document will be attached to the data to provide more detailed information.

- **Pain Face Prediction Task**: The aim of this task is to build a classification/prediction model to differentiate between a participant with CLBP and a healthy control participant as well as continuously recognise the levels of observer-rated pain of participants with CLBP, based on facial expression during exercise performance. We provide training, validation, and test data, which comprise features extracted from face video data from both participants with CLBP and healthy control participants. Participants should see below for details about these data, and how to access the data for this task. A README document will be attached to the data to provide more detailed information.



## Dataset

- **Joint Angles** and **Joint Energies** (calculated from the joint angles). See diagram below, taken from [Wang et al. 2019b](https://arxiv.org/abs/1904.10824):

<p align="center">
<img width="300" height="240" src="images/Angle.PNG">
</p>

- **sEMG data**. The data given is the upper envelope of the rectified sEMG sensor data. See diagram on left below for the placement of the sensors, taken from [Aung et al. 2016](https://ieeexplore.ieee.org/abstract/document/7173007)

<p align="center">
<img width="160" height="240" src="images/sEMGcapture.PNG">
</p>


- **Facial geometric feature plus deep feature** This includes facial landmarks, head pose, HOG, action unit occurrence and intensity values extracted from [OpenFace](https://github.com/TadasBaltrusaitis/OpenFace), and deep-learned feature representations.Figure below shows the detailed description and the dimensions of the facial expression data.


<p align="center">
<img width="400" height="308" src="images/facefeature2.png">
</p>

## Dataset Partition
The movement dataset is divided randomly into 
- Training Set (10 CLBP participants, 6 healthy participants)
- Validation Set (4 CLBP participants, 3 healhy participants)
- Test Set (3 CLBP participants, 5 healhy participants)

The face dataset is divided randomly into 
- Training Set (8 CLBP participants, 11 healthy participants)
- Validation Set (3 CLBP participants, 6 healhy participants)
- Test Set (3 CLBP participants, 5 healhy participants)

## Participate
To participate in the EmoPain Challenge 2019, please download, fill, and sign the EULA (link coming soon). The form should then be sent to **emopain19@gmail.com**.
<br>

When we receive the form, the link to the training and validation sets will be emailed to the sender. At a later date, the link to the test set will also be forwarded.
<br>
The test set results should be sent by each participating team to the email address above. Each team can submit up to 5 different results. 
<br>
The test results performance ranking will be based on the metric described below. The ranking over all will be displayed on this website, before the workshop day.

## Metric
- For the Movement Behaviour Classification and the Pain Recognition from Movement tasks, we will use the mean F1 score as the performance metric:

<p align="center">
<img width="272" height="64" src="images/meanf1.PNG">
</p>

where _pre_ and _recall_ are the precision and recall ratios respectively of class _c_.

- For the task on face, Mean Sqaure Error (MSE), Mean Absolute Error (MAE), Pearson Coreelation Coefficient (PCC) and Concordance Correlation Coefficient (CCC) will be used.

## Paper Submission
Papers should be up to 7 pages (6 pages + 1 page for references) and submitted through EasyChair (link coming soon). Please see below for dates. The reviewing process will be double-blind.
<br>

## Important Dates (Postponed, more information coming soon)

- Training and Validation Data Available: 28th of June, 2019
- Testing Data Available: 3th of July, 2019 
- Results Uploading Deadline: 7th of July, 2019
- Paper Submission Deadline: 10th of July 2019
- Notification: 15th of July 2019 
- Camera Ready due: 19th of July, 2019 
- Workshop Date: 3rd of September, 2019

## Organisers
### General Chairs
Prof Nadia Berthouze, UCL
Dr. Amanda Williams, UCL
Dr Michel Valstar, University of Nottingham
Dr Hongying Meng, Brunel University London
Dr Min Aung, University of East Anglia
Dr Nicholas Lane, University of Oxford

### Data Chairs
Dr Joy Egede, University of Nottingham
Dr Olugbade Temitayo, UCL
Chongyang Wang, UCL
Siyang Song, University of Nottingham

## Keynote Speakers

#### [Professor Rebecca Slater, Oxford University, UK (tentative)](https://www.paediatrics.ox.ac.uk/team/rebeccah-slater)
#### [Professor Chris Eccleston, University of Bath, UK (tentative)](https://researchportal.bath.ac.uk/en/persons/chris-eccleston)

We also aim to have a multidisciplinary panel (in line with the inclusion theme of ACII 2019) on the requirements and challenges from 
real world applications for the above-discussed technology.
<br>
We hope that the discussion will trigger interest that leads to new approaches for developing automatic recognition systems. 
<br>
The panel will be led by a member of the organizing committee (Dr Amanda Williams, clinical psychologist and academic expert in pain) and include 2 keynote speakers (see above), a senior physiotherapist (Mr Diarmuid Denneny, Pain Management Centre, UCLH NHS Foundation Trust, UK) and an HCI researcher (Dr Aneesha Singh, UCL, with long-term research experience with pain patients).
