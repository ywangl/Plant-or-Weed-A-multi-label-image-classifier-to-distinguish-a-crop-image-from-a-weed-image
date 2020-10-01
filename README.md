# Plant or Weed: A multi label image classifier to distinguish a crop image from a weed image

![5e713b8a74460 image](https://user-images.githubusercontent.com/66754032/94639081-044bd180-02a1-11eb-9922-391bc4d1f25b.jpg)

# Can you differentiate a weed from a crop seedling?

The ability to do so effectively can mean better crop yields and better stewardship of the environment.

This was our final Data Mining presentation at the University of Chicago!(Team: [Aakash](https://www.linkedin.com/in/aakash-pahuja16/), [Adrienne](https://www.linkedin.com/in/adrienneywang/), Murphy, [Nara](https://www.linkedin.com/in/narasimha-kamath-ardi-133169132/), [Rupa](https://www.linkedin.com/in/satarupa-ghosh-pmp-1413634/), [Xintian](https://www.linkedin.com/in/xintiansu/))

Followed by basic statistical summary of our dataset, we further explored our data after transformation into a 4750X16384 matrix using tSNE, Hierarchical Clustering, DBSCAN, and K-means clustering. Although some seedling categories had more images than others, we didn't balance our data using KDE to generate more images because by using the last layer of CNN, imbalanced data won't be problematic. (Check slide number 10 to see the stops of using KDE to generate images)

We are using OpenCV to create image masks(just to show how to use OpenCV). In addition, we are tarining our models using CNNs. 

The last layer of the CNN(dense layer) is fed into other models like SVM and Random Forest to check how other models behave in classifiying the seedlings!

We also played with CNN models with different layers. (Inception v3, Xception and VGG19)

Current work: We are working on developing a web application using Flask! In addition, we will then deploy our application on Heroku.

Please check for regular updates as the repository can keep changing, especially the web application portion of the project.

You can access the datasets here: https://www.kaggle.com/c/plant-seedlings-classification

Happy Coding!


Notice: CNN+SVM gave the highest accuracy score but it is overfitting, thus not selected. Validation performance is not ideal on google searched images. 
