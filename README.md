# Solution of Team IMR for MICCAI 2023 AIIB Challenge

[**_USNet: Universal-Specific Network for Airway Modeling of Pulmonary Fibrosis CT Scans_**]()

> By Minghui Zhang, Hanxiao Zhang, Yangqian Wu, and Yun Gu
>> Institute of Medical Robotics, Shanghai Jiao Tong University


## Dataset
The dataset could be obtained from [here](https://codalab.lisn.upsaclay.fr/competitions/13238#learn_the_details-dataset).


## Usage
The docker of our method can be downloaded by [Google Drive Link](https://drive.google.com/file/d/1l76Yym8RFwc4kZ0Sq2RSux5fq7bqat-M/view?usp=sharing) 

Step 1, please load our docker from the compressed file:

```
docker image load < imrv1.tar.gz
```

Step 2, we have followed your tutorial with slight change, please use the following to run our docker:

```
docker container run --gpus "device=0" --name imrv1 --rm -v [input directory]:/input -v [output directory]:/output imrv1:latest
```