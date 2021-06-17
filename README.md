# Unbiased Mobility Data with Preferential Sampling
** Hosted by **: The Data Science for Social Good (DSSG) program at the University of British Columbia
** Sponsor **: Cedar Academy Society
** Description **: Public sector and academic communities have been using mobility and traffic data as a proxy measurement for a variety of social topics, from GDP prediction and economic development to greenhouse gas emissions and environmental impact. One method to measure mobility and acquire traffic data is through the analysis of pictures and footage from traffic cameras installed at fixed locations (in urban and rural areas). More often than not, the cameras are installed near locations with heavy traffic, and this introduces sampling bias in the observed data. This leads to a biased dataset and overexaggerates nearby mobility levels due to “preferential sampling.” This project seeks to correct this preferential sampling and develop an algorithm to better model mobility levels while accounting for the bias in the data set.


### Data:
*The followig is untampered, full-YOLOv3-extracted raw information in the data file. For that reason, please ignore the "MOV index" part (this is for clients who need aggregated and scaled data) in the user's guide. 

  * Data description: https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/Surrey_desc.csv - automatic!
  * Data file: https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/Surrey_data.csv - automatic!
  * User's guide: https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/VanCom_Mobility_Data_User's_Guide_1.2.pdf - automatic!

* Hourly snapshots jpeg files from two camera stations have been pulled and stored below for your reference. The two station are
  * 104 Ave And 140 St (station name: enc_104_140_cam1) https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/dssg_jpg_1.zip - automatic!
  * 104 Ave And City Hall Driveway (station name: enc_104egress_cityhall_cam1) https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/dssg_jpg_2.zip - automatic!

* Interesting datasets on the City of Surrey here: 
https://data.surrey.ca/dataset
and its 2015 Traffic Counts dataset:
https://data.surrey.ca/dataset/traffic-counts-2015 - automatic!
https://data.surrey.ca/dataset/traffic-signals  - automatic! (not all traffic signal location will have cameras etc.)
https://data.surrey.ca/dataset/traffic-volumes - automatic!

* StatCan boundary data (.shp file): 
https://5rv1kcdhjldl7wjmwwrxqd.s3-us-west-2.amazonaws.com/lfsa000b16a_e.zip - automatic!

* Two links that can give you inspiration of how to get information about the "features" of an intersection 
https://towardsdatascience.com/openstreetmap-from-browser-querying-to-python-r-manipulation-c8e4504ad709  - automatic!
https://www.r-bloggers.com/2020/08/geocoding-an-intersection-with-open-street-map-data/ - automatic!

* Image pre-processing:
Gamma correction or histogram transformations. Some examples are here:
https://scikit-image.org/docs/dev/api/skimage.exposure.html - automatic!

### Potential Pathways:
1. Mobility data in real estate context
https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3770895 - automatic!
in Canadian Economics Society Annual Meeting 2021
https://cea2021.exordo.com/programme/presentation/631 - automatic!

2. Object recognition in crowd / Crowd Classifier

3. GHG emission indexing
I was referring to here: https://github.com/foamliu/Car-Recognition - automatic!
and a Standford car dataset here: http://ai.stanford.edu/~jkrause/cars/car_dataset.html - automatic!

4. Crime Prevention
Minority Report kind of Crime Prevention research here:
https://ojs.aaai.org//index.php/ICWSM/article/view/7304 - automatic!


### Recent Update:
* Partnership with industry leader SafeGraph:
Placekey + VanCom: Combining Anonymized Traffic Activity Datasets and POI Data for Advanced Analytics
https://www.placekey.io/blog/placekey-vancom - automatic!

### Related Projects:
1. Neurips 2021’s competition Traffic4cast:
https://www.iarai.ac.at/traffic4cast/ - automatic!
2. Android smartphones high accuracy GNSS datasets
https://www.kaggle.com/google/android-smartphones-high-accuracy-datasets?select=ION+GNSS+2020+Android+Raw+GNSS+Measurement+Datasets+for+Precise+Positioning.pdf - automatic!



### References:

Understanding Traffic Density from Large-Scale Web Camera Data, Shanghang Zhang, Guanhang Wu, João P. Costeira, José M. F. Moura, arXiv:1703.05868 [cs.CV]

A general theory for preferential sampling in environmental networks, Watson, J, V. Zidek, J, Shaddick, G, Annals of Applied Statistics, 2019, 2662-2700

Object Counting on Low Quality Images: A Case Study of Near Real-Time Traffic Monitoring, Jean-Francois Rajotte, Martin Sotir, Cedric Noiseux, Louis-Philippe Noel, Thomas Bertiere, IEEE Xplore: 17, January 2019






