# Unbiased Mobility Data Project

**Hosted by**: [The Data Science for Social Good (DSSG) program](https://dsi.ubc.ca/data-science-social-good#projects) at the [University of British Columbia](https://www.ubc.ca/)

**Sponsor**: Cedar Academy Society - [VanCom Project](https://data.pwfh.org/)

**Time**: May 2021 - August 2021

**Description**: Public sector and academic communities have been using mobility and traffic data as a proxy measurement for a variety of social topics, from GDP prediction and economic development to greenhouse gas emissions and environmental impact. One method to measure mobility and acquire traffic data is through the analysis of pictures and footage from traffic cameras installed at fixed locations (in urban and rural areas). More often than not, the cameras are installed near locations with heavy traffic, and this introduces sampling bias in the observed data. This leads to a biased dataset and overexaggerates nearby mobility levels due to “preferential sampling.” This project seeks to correct this preferential sampling and develop an algorithm to better model mobility levels while accounting for the bias in the data set.



### Data:
Request for download link at <ins> data@pwfh.org</ins>, for data items with this ![in red](https://via.placeholder.com/15/f03c15/000000?text=+) 

Click to download a high-level [VanCom Mobility Data Users' Guide.](https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/VanCom_Mobility_Data_User's_Guide_1.2.pdf)

**Data from Cedar Academy Society:**
1. ![in red](https://via.placeholder.com/15/f03c15/000000?text=+) Main Dataset 
   
   Time: December 1-31, 2020
   
   Assets: 364 location-based Assets in the City of Surrey, British Columbia, Canada

   [![map](https://s3.amazonaws.com/data.pwfh.org/ubcdssg/pic1.png)](https://api.mapbox.com/styles/v1/scotthughes/ckq7op9qz5zom17pj0pcv2y83.html?fresh=true&access_token=pk.eyJ1Ijoic2NvdHRodWdoZXMiLCJhIjoiY2p3bWg5OTc5MGJ0NzRha2VlbXFtOTZheSJ9.c4EyzyAn28dXg3HujMoarg#10.01/49.112/-122.7691)

   Description: The file contains full-YOLOv3-extracted information from raw static image files. For that reason, please ignore the "MOV index" part (this is for clients who need aggregated and scaled data) in the Users' Guide. 

  * Data Description file screenshot![Data description:](https://s3.amazonaws.com/data.pwfh.org/ubcdssg/pic2.png)
  * Data file screenshot![Data file:](https://s3.amazonaws.com/data.pwfh.org/ubcdssg/pic2.png)


2. ![in red](https://via.placeholder.com/15/f03c15/000000?text=+) 60 min-gap raw images
   
   JPEG files from two camera stations have been pulled and stored below for your reference
   
   Time: December 1-31, 2020
   
   Assets: 2 location-based Assets in the City of Surrey
      * 104 Ave And 140 St
      * 104 Ave And City Hall Driveway


| 104 Ave And 140 St(station name: enc_104_140_cam1)| 104 Ave And City Hall Driveway(station name: enc_104egress_cityhall_cam1) |
| :---         |     :---:      |
| ![](https://s3.amazonaws.com/data.pwfh.org/ubcdssg/pic4.png)   | ![](https://s3.amazonaws.com/data.pwfh.org/ubcdssg/pic5.png)     | 

3. ![in red](https://via.placeholder.com/15/f03c15/000000?text=+) 15 min-gap extract data

   Time: October 10-16, 2020
   
   Assets: 364 location-based Assets in the City of Surrey, British Columbia, Canada

4. ![in red](https://via.placeholder.com/15/f03c15/000000?text=+) 2 min-gap raw images

   Time: May 2-3, 2020
   
   Asset: 1 location-based Asset: 104 Ave And 140 St


**Data and tools from other sources:**
* [Interesting datasets](https://data.surrey.ca/dataset) on the City of Surrey here 
  
  and Surrey 2015 [Traffic Counts dataset](https://data.surrey.ca/dataset/traffic-counts-2015)

  Not all traffic signal location will have [cameras](https://data.surrey.ca/dataset/traffic-signals)

* [StatCan boundary data (.shp file):](https://www12.statcan.gc.ca/census-recensement/2011/geo/bound-limit/bound-limit-eng.cfm)
  
  [Road network in Surrey](https://data.surrey.ca/dataset?q=road&sort=score+desc%2C+metadata_modified+desc) and from [DataBC](https://catalogue.data.gov.bc.ca/dataset?q=road)
  
* Geocoding tools:

  The following links that can give you inspiration of how to get information about the "features" of an intersection
  
  * [OpenStreetMap: From Browser Querying to Python+R Manipulation](https://towardsdatascience.com/openstreetmap-from-browser-querying-to-python-r-manipulation-c8e4504ad709)
  * [Geocoding An Intersection with Open Street Map data](https://www.r-bloggers.com/2020/08/geocoding-an-intersection-with-open-street-map-data/)
  * [DataBC GeoCoder API](https://www2.gov.bc.ca/gov/content/data/geographic-data-services/location-services/geocoder)

<strike>
### Sample Code:
##### Requirements
* os
* datetime
* pandas
* json
* time
* numpy
* geopandas
##### [coming soon] ....
</strike>

### Potential Directions:
##### Applications
1. Traffic prediction. A survey can be found [here](https://arxiv.org/abs/1908.10218) [[9]](#9)

2. [Mobility data in Real Estate](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3770895) context
and [Canadian Economics Society Annual Meeting 2021 presentation](https://cea2021.exordo.com/programme/presentation/631)

3. <strike>GHG emission indexing</strike>

   The idea is to project vehicle type/make recognition to Green House Gas emission. A starting point can be car recognition mechanism from image/video files, e.g., [here on Github](https://github.com/foamliu/Car-Recognition)

   and a [Standford car dataset here](http://ai.stanford.edu/~jkrause/cars/car_dataset.html). 
    
   The challenge in this case is the low resolution of raw image/video files that makes ID of vehicles logo and shape of headlights impossible. 

4. Crime Prevention [[7]](#7)

   The idea is a [**_Minority Report_** kind of mechanism](https://ojs.aaai.org//index.php/ICWSM/article/view/7304)

5. Economic Recovery post Pandemic [[4]](#4)
    
    [Mobility and Engagement Index](https://www.dallasfed.org/research/mei) by the Federal Reserve Bank of Dallas
   
    [The Impact of COVID-19 on Small Business Dynamics and Employment](http://www.andrekurmann.com/hb_covid)
    
    [Bloomberg article: High-Frequency Data Prove Their Staying Power With Fed’s Buy-In](https://www.bloomberg.com/news/articles/2020-09-15/high-frequency-data-prove-their-staying-power-with-fed-s-buy-in)

6. Weather influence on Mobility

7. Bike routes monitoring


| Cam and Shared Traffic| Cam and Bike Lanes |
| :---         |     :---:      |
| <img src="https://s3.amazonaws.com/data.pwfh.org/ubcdssg/overlay+of+cam+and+Shared+Traffic.png" width="200" height="150">   | <img src="https://s3.amazonaws.com/data.pwfh.org/ubcdssg/overlay+of+cam+and+Bike+Lanes.png" width="300" height="150">  | 


##### Infrastructure
1. Bias correction

2. Metadata
   
3. Better Object Detection
   * Crowd Counting / Crowd Classifier [[1]](#1)
   * Rolling window
   * [Background Subtraction](https://docs.opencv.org/3.4/d1/dc5/tutorial_background_subtraction.html) with OpenCV and a comprehensive intro [here](https://sites.google.com/site/backgroundsubtraction/test-sequences)
   * YOLOv3 --> YOLOv4 --> [YOLOv5](https://github.com/ultralytics/yolov5), [PAFNet](https://paperswithcode.com/paper/pafnet-an-efficient-anchor-free-object), Rotate Anchor, [PaddleDetection](https://github.com/PaddlePaddle/PaddleDetection)
   * Image pre-processing
     
     Gamma correction or histogram transformations. [Some examples are here:](https://scikit-image.org/docs/dev/api/skimage.exposure.html)
   * CV model trained on traffic camera datasets [[6]](#6)
     
     [STREET dataset](https://databank.illinois.edu/datasets/IDB-3671567)
   * Try [Yolov5](https://github.com/ultralytics/yolov5)
    
   Linux, inference with detect.py 
   ```
   # clone github repo
    git clone https://github.com/ultralytics/yolov5.git
    
    # clear requirements and download pretrained model weights
    cd yolov5
    
    pip install -r requirements.txt
    
    python detect.py --weights yolov5s.pt
    python detect.py --weights yolov5m.pt
    python detect.py --weights yolov5l.pt
    python detect.py --weights yolov5x.pt
    
    # Try Yolov5 on static image files
    
    python detect.py --source 2020-12-06-23-22-42-enc_104_140_cam1.jpg --weights yolov5s.pt --project infer_yolov5s_2
    
    python detect.py --source 2020-12-06-23-22-42-enc_104_140_cam1.jpg --weights yolov5x.pt --project infer_yolov5s_3

   ```
   
   * Try [PaddleSeg](https://github.com/PaddlePaddle/PaddleSeg) for Semantic Segmentation
    
   [AutoNue Challenge](http://cvit.iiit.ac.in/autonue2021/challenge/) 1st Prize Winner at CVPR 2021
    
   
4. Edge Computing
   * Using edge device to extract traffic insights [[3]](#3)
     
     for example, [Papers with Code - Mobile Video Object Detection with Temporally-Aware Feature Maps](https://paperswithcode.com/paper/mobile-video-object-detection-with-temporally)
   * See Microsoft [Project Rocket](https://www.microsoft.com/en-us/research/project/live-video-analytics/) for [Vision Zero](https://en.wikipedia.org/wiki/Vision_Zero) -related projects insight

5. Hardware

   * [ESP32](http://esp32.net/) and ESP32-CAM

6. Scalable Object Detection Pipeline
    
   * NVIDIA, Deploying a Scalable Object Detection Inference Pipeline [Blog: Intro](https://developer.nvidia.com/blog/deploying-a-scalable-object-detection-inference-pipeline/)
   * NVIDIA, Deploying a Scalable Object Detection Inference Pipeline [Blog: The Inferencing Process](https://developer.nvidia.com/blog/deploying-a-scalable-object-detection-pipeline-the-inferencing-process-part-2/)

7. [PaddleDetection](https://github.com/PaddlePaddle/PaddleDetection)
<img src="https://s3.amazonaws.com/data.pwfh.org/ubcdssg/fps_map_pp_detection.png">

### Recent Update:
* VanCom partnership with industry leader SafeGraph:
[Placekey + VanCom: Combining Anonymized Traffic Activity Datasets and POI Data for Advanced Analytics](https://www.placekey.io/blog/placekey-vancom)



### Related Projects, Datasets, and Repositories:
1. NeurIPS 2021’s competition [Traffic4cast](https://www.iarai.ac.at/traffic4cast/)
2. Kaggle's Android smartphones high accuracy [GNSS datasets](https://www.kaggle.com/google/android-smartphones-high-accuracy-datasets?select=ION+GNSS+2020+Android+Raw+GNSS+Measurement+Datasets+for+Precise+Positioning.pdf)
3. Standford car (type/make) dataset [here](http://ai.stanford.edu/~jkrause/cars/car_dataset.html)
4. [UA-DETRAC](https://detrac-db.rit.albany.edu/) dataset (detection/tracking), with research paper here [[8]](#8)
5. [CVOnline - Compendium of Computer Vision](https://homepages.inf.ed.ac.uk/rbf/CVonline/Imagedbase.htm)
6. NVidia [AI CITY CHALLENGE](https://www.aicitychallenge.org/)
### References:

<a id="1">[1]</a> Understanding Traffic Density from Large-Scale Web Camera Data, Shanghang Zhang, Guanhang Wu, João P. Costeira, José M. F. Moura, arXiv:1703.05868 [cs.CV]

<a id="2">[2]</a> A general theory for preferential sampling in environmental networks, Watson, J, V. Zidek, J, Shaddick, G, Annals of Applied Statistics, 2019, 2662-2700

<a id="3">[3]</a> Object Counting on Low Quality Images: A Case Study of Near Real-Time Traffic Monitoring, Jean-Francois Rajotte, Martin Sotir, Cedric Noiseux, Louis-Philippe Noel, Thomas Bertiere, IEEE Xplore: 17, January 2019

<a id="4">[4]</a> Mobility and Engagement Following the SARS-Cov-2 Outbreak, the Federal Reserve Bank of Dallas

<a id="5">[5]</a> Leveraging Administrative Data for Bias Audits: Assessing Disparate Coverage with Mobility Data for COVID-19 Policy, Amanda Coston, Neel Guha, Derek Ouyang, Lisa Lu, Alexandra Chouldechova, Proceedings of the 2021 ACM Conference on Fairness, Accountability, and Transparency. pp. 173-184, arXiv:2011.07194 [stat.AP]

<a id="6">[6]</a> STREETS: A Novel Camera Network Dataset for Traffic Flow, Advances in Neural Information Processing Systems 32 (NeurIPS 2019)

<a id="7">[7]</a> Leveraging Mobility Flows from Location Technology Platforms to Test Crime Pattern Theory in Large Cities, Cristina Kadar, Stefan Feuerriegel, Anastasios Noulas, Cecilia Mascolo, arXiv:2004.08263 [cs.CY]

<a id="8">[8]</a> UA-DETRAC: A New Benchmark and Protocol for Multi-Object Detection and Tracking, Longyin Wen, Dawei Du, Zhaowei Cai, Zhen Lei, Ming-Ching Chang, Honggang Qi, Jongwoo Lim, Ming-Hsuan Yang, Siwei Lyu, 2020, arXiv:1511.04136 [cs.CV]

<a id="9">[9]</a> Urban flows prediction from spatial-temporal data using machine learning: A survey, 	arXiv:1908.10218 [cs.LG]
