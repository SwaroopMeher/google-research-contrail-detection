# google-research-contrail-detection [ICRGW] <br>

Contrails are clouds of ice crystals that form in aircraft engine exhaust. These contrails have the potential to contribute to global warming by trapping heat within the Earth's atmosphere. To better understand and address this issue, researchers have created models that can predict the occurrence of contrails and estimate the extent to which they contribute to warming. However, in order to validate these models, the researchers require satellite imagery.<br>
<br>
The ICRGW aims to utilize satellite imagery to identify contrails produced by airplanes. It employs segmentation, which involves separating the contrails from the rest of the image using a mask. By solving this segmentation problem, the project can accurately pinpoint the contrails within the satellite images. This work will quantifiably improve the confidence in prediction of contrail forming regions by the models build by researchers and the techniques to avoid creating them.<br>

The success of this project can be assessed on two factors. Firstly, the development of an ML pipeline that effortlessly generates precise segmentation masks from any input image. 
Secondly, to model successfully segments ~1800 images, with an impressive dice coefficient of greater than 0.6 on the hidden test set on Kaggle leaderboard. <br>

#Results:<br>
![image](https://github.com/SwaroopMeher/google-research-contrail-detection/assets/115743490/ca7b6172-776a-4d4b-b9fa-66ea3a3a250e)
<br>

#Data sources:<br>
This project uses geostationary satellite images to identify aviation contrails. The original satellite images were obtained from the NASA’s GOES-16 Advanced Baseline Imager (ABI) [1]. 
These satellite images were then manually labeled and combined into a dataset with temporal context as explained by the authors of the paper OpenContrails: Benchmarking Contrail Detection on GOES-16 ABI [2]. <br>
The dataset is available on Kaggle [3]. It has 20,529 train records, 1,826 validation records and ~1,800 test records. Each record has satellite images in 8 bands and a human labelled segmentation mask [3].

#References:<br>
[1] GOES-16 Advanced Baseline Imager - https://www.goes-r.gov/spacesegment/abi.html<br>
[2] https://arxiv.org/abs/2304.02122<br>
[3] https://www.kaggle.com/competitions/google-research-identify-contrails-reduce-global-warming/data<br>

<br>Please check the powerpoint presentation and the code for more info.






