# CSEIDLProject
CSEIDLProject

This project deals with classification of musculoskeletal radiographs into abnormal and normal. In this project we worked on 6 models, namely, VGG16, ResNet50, DenseNet169, NasNetLarge, NasNet trained from scratch and InceptionV3 model. We have compared these models using recall, accuracy and precision and analyzed them so as to which model performed better and why. The complete results and analysis is in the report.

As the data from MURA is very large we have segregated it into seperate csv files for each arm part namely, Train_set_ELBOW.csv, Train_set_FINGER.csv, Train_set_FOREARM.csv, Train_set_HAND.csv, Train_set_HUMERUS.csv, Train_set_SHOULDER.csv and Train_set_WRIST.csv. Since these files are huge we could not upload them in Canvas or github. Therefore we have included the code where we are creating these files from the main dataset. This is done in muracam.ipynb file. Once this file we will have all the seperate csv files containing the required data to run individual models.

Further one has to decide which model they want to run among the files NasNet.ipynb, vgg.ipynb, resnet.ipynb, inception.ipynb, densenet.ipynb and nasnet_train.ipynb and for which body part. Once model is decided they have to open the particular model file from the submitted ones and run it for particular body part(to be selected within the code). The code will print out the performance metrics in the end of the file. We have ran our code in Agave clusters as running them in CPU will take a lot of time and might crash in between. Below are the configurations with which we ran our code-

GPU -  1 NVIDIA Tesla V100 SXM2 16 GB 
CPU - Intel® Xeon® Processor E5-2650 v4 12
Cores per socket - 12
Threads per core - 1 
Sockets -2 
CPU MHz - 1562.854
CPU max MHz - 2200
CPU min MHz - 1200
Memory - 8 GB

Once the classification is done one can localize the abnormality in particular image using the muracam.ipynb file. We have also included the results screenshots for individual arm part and model in folders of submitted zip file.
We have also added one requirements.txt file which summarises the required libraries for running this project.

