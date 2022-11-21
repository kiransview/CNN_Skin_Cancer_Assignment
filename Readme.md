# Melanoma Skin Cancer Detection via CNN Assignement
##Problem Statement:
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

The data set contains the following diseases:

Actinic keratosis, Basal cell carcinoma, Dermatofibroma, Melanoma, Nevus, Pigmented benign keratosis, Seborrheic keratosis, Squamous cell carcinoma, Vascular lesion

##Process followed

1. Train & Val Data Split for accuracy measurement (model Improvement).
2. Initial EDA before Building a Model.
3. Based on simple Sequential Model with 20 ephocs we got an accuracy of Training - 90% & Val - 54% - Model Tend to Overfit.
![image](https://user-images.githubusercontent.com/61668526/203008776-b32d270a-70f2-4099-ab1d-b470dc42df11.png)
4. Implemented Data Augmentaion strategy by using some Augmentation techniques.
5. EDA of the same data to understand the compositon of the data images.
6. Based on same simple Sequential Model with 50 ephocs & the data augmented we got an accuracy of Training - 81% & Val - 64% - Model Tend to similarly overfit.
![image](https://user-images.githubusercontent.com/61668526/203009484-7e825d73-cfc0-4314-8ab9-ccf9416b58ae.png)
7. With the same utilization of the model with some addition of dropout layes model had a accuracy of Training - 91% & Val - 51% .
![image](https://user-images.githubusercontent.com/61668526/203009820-987f51ca-2bf7-44d1-9320-3fefa2335b6f.png)
8. As the final step gone with data reblancing for better performance.
9. Below is the list of samples in each class.
![image](https://user-images.githubusercontent.com/61668526/203010106-4918f060-9f8f-453d-b0dd-6f7d051822a2.png)
10. As we can see a clear imbalance lets try to balance by upscaling the data to 500 (Augmentor Library Used for processing).
11. Based on the sequential model with some changes in the layers by adding and removing some layers. the accuracy of Training - 91% & Val - 80% - Model Tend to perform better based on the improvement in the scaling.
![image](https://user-images.githubusercontent.com/61668526/203010779-32c935ca-a5c5-4a24-8b4c-06798918f0f6.png)
12. So to furhter tune the model we can use Hyperparameter on the ephocs, optimizers...etc.

