# Unbiased Mobility Data Project

**Hosted by**: [The Data Science for Social Good (DSSG) program](https://dsi.ubc.ca/data-science-social-good) at the [University of British Columbia](https://www.ubc.ca/)

**Sponsor**: Cedar Academy Society - [VanCom Project](https://data.pwfh.org/)

**Description**: Public sector and academic communities have been using mobility and traffic data as a proxy measurement for a variety of social topics, from GDP prediction and economic development to greenhouse gas emissions and environmental impact. One method to measure mobility and acquire traffic data is through the analysis of pictures and footage from traffic cameras installed at fixed locations (in urban and rural areas). More often than not, the cameras are installed near locations with heavy traffic, and this introduces sampling bias in the observed data. This leads to a biased dataset and overexaggerates nearby mobility levels due to “preferential sampling.” This project seeks to correct this preferential sampling and develop an algorithm to better model mobility levels while accounting for the bias in the data set.



### Data:
* The following is untampered, full-YOLOv3-extracted raw information in the data file. For that reason, please ignore the "MOV index" part (this is for clients who need aggregated and scaled data) in the user's guide. 

  * [Data description:](https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/Surrey_desc.csv)
  * [Data file:](https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/Surrey_data.csv)
  * [User's guide:](https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/VanCom_Mobility_Data_User's_Guide_1.2.pdf)

* Hourly snapshots jpeg files from two camera stations have been pulled and stored below for your reference. The two station are
  * [104 Ave And 140 St (station name: enc_104_140_cam1)](https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/dssg_jpg_1.zip)
  * [104 Ave And City Hall Driveway (station name: enc_104egress_cityhall_cam1)](https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/dssg_jpg_2.zip)

* [Interesting datasets on the City of Surrey here:](https://data.surrey.ca/dataset) 
[and its 2015 Traffic Counts dataset:](https://data.surrey.ca/dataset/traffic-counts-2015)
[Not all traffic signal location will have cameras](https://data.surrey.ca/dataset/traffic-signals)

* [StatCan boundary data (.shp file):](https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/lfsa000b16a_e.zip)
  [Road network in Surrey](https://data.surrey.ca/dataset?q=road&sort=score+desc%2C+metadata_modified+desc) and from [DataBC](https://catalogue.data.gov.bc.ca/dataset?q=road)

* Geocoding:
Two links that can give you inspiration of how to get information about the "features" of an intersection 
[OpenStreetMap: From Browser Querying to Python+R Manipulation](https://towardsdatascience.com/openstreetmap-from-browser-querying-to-python-r-manipulation-c8e4504ad709)
[Geocoding An Intersection with Open Street Map data](https://www.r-bloggers.com/2020/08/geocoding-an-intersection-with-open-street-map-data/)
[DataBc GeoCoder API](https://www2.gov.bc.ca/gov/content/data/geographic-data-services/location-services/geocoder)

### Potential Directions:
##### Application
1. [Mobility data in Real Estate context](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3770895)
and [Canadian Economics Society Annual Meeting 2021 presentation](https://cea2021.exordo.com/programme/presentation/631)

2. GHG emission indexing
[I was referring to here:](https://github.com/foamliu/Car-Recognition)
and a [Standford car dataset here:](http://ai.stanford.edu/~jkrause/cars/car_dataset.html)

3. Crime Prevention
[**_Minority Report_** kind of Crime Prevention research here:](https://ojs.aaai.org//index.php/ICWSM/article/view/7304)

4. Economic Recovery post Pandemic
   [Mobility and Engagement Index](https://www.dallasfed.org/research/mei) by the Federal Reserve Bank of Dallas
   [Bloomberg article: High-Frequency Data Prove Their Staying Power With Fed’s Buy-In](https://www.bloomberg.com/news/articles/2020-09-15/high-frequency-data-prove-their-staying-power-with-fed-s-buy-in)

5. Weather influence on Mobility

##### Infrastructure
1. Better Object ID
   * Object recognition in crowd / Crowd Classifier
   * YOLOv3 --> YOLOv4 --> [YOLOv5](https://github.com/ultralytics/yolov5), [PAFNet](https://paperswithcode.com/paper/pafnet-an-efficient-anchor-free-object), Rotate Anchor, [PaddleDetection](https://github.com/PaddlePaddle/PaddleDetection)
   * Image pre-processing
     [Gamma correction or histogram transformations. Some examples are here:](https://scikit-image.org/docs/dev/api/skimage.exposure.html)
   * CV model trained on traffic camera datasets
     [STREET dataset](https://databank.illinois.edu/datasets/IDB-3671567)

2. Edge Computing
   * Using edge device to extract traffic insights
     for example, [Papers with Code - Mobile Video Object Detection with Temporally-Aware Feature Maps](https://paperswithcode.com/paper/mobile-video-object-detection-with-temporally)


### Recent Update:
* Partnership with industry leader SafeGraph:
[Placekey + VanCom: Combining Anonymized Traffic Activity Datasets and POI Data for Advanced Analytics](https://www.placekey.io/blog/placekey-vancom)



### Related Projects:
1. [Neurips 2021’s competition Traffic4cast:](https://www.iarai.ac.at/traffic4cast/)
2. [Android smartphones high accuracy GNSS datasets](https://www.kaggle.com/google/android-smartphones-high-accuracy-datasets?select=ION+GNSS+2020+Android+Raw+GNSS+Measurement+Datasets+for+Precise+Positioning.pdf)



### References:

Understanding Traffic Density from Large-Scale Web Camera Data, Shanghang Zhang, Guanhang Wu, João P. Costeira, José M. F. Moura, arXiv:1703.05868 [cs.CV]

A general theory for preferential sampling in environmental networks, Watson, J, V. Zidek, J, Shaddick, G, Annals of Applied Statistics, 2019, 2662-2700

Object Counting on Low Quality Images: A Case Study of Near Real-Time Traffic Monitoring, Jean-Francois Rajotte, Martin Sotir, Cedric Noiseux, Louis-Philippe Noel, Thomas Bertiere, IEEE Xplore: 17, January 2019

Mobility and Engagement Following the SARS-Cov-2 Outbreak, the Federal Reserve Bank of Dallas

Leveraging Administrative Data for Bias Audits: Assessing Disparate Coverage with Mobility Data for COVID-19 Policy, Amanda Coston, Neel Guha, Derek Ouyang, Lisa Lu, Alexandra Chouldechova, Proceedings of the 2021 ACM Conference on Fairness, Accountability, and Transparency. pp. 173-184, arXiv:2011.07194 [stat.AP]

STREETS: A Novel Camera Network Dataset for Traffic Flow, Advances in Neural Information Processing Systems 32 (NeurIPS 2019)


