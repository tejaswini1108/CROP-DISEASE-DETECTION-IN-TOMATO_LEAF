# CROP-DISEASE-DETECTION-IN-TOMATO_LEAF
The quality and quantity of the crop are significantly affected by numerous diseases in plants. In this regard, an early detection of such diseases is highly effective. Tomato is one of the important crops that is produced in large quantities with high commercial value. Diseases harm the health of theplant, which has an impact on its growth. It is critical to monitor the progress of the farmed crop toguarantee minimal losses.
There are different types of tomato diseases. One of the major linkages in the avoidance and control of crop diseases is the identification of infections in the leaf portions during the planting phase. Tomato leaves, including nine popular species(Bacterial Spot, Early Blight, Late Blight, Mosaic Virus, and Septoria Spot,yellow curl,target_spot,two spotted_spidermite), are used as experimental objects in this work to extract disease features from the leaf surface. Deep learning based disease identification might help prevent such a catastrophe. A Convolutional Neural Network(CNN) is a type of deep learning algorithm that is currently used for image categorization.We used the CNN architecture to identify diseases in tomato leaves.

## DATA SET
Our dataset is divided into three sets: train, test, and validation. Each folder has 10 subfolders labelled "plant diseases," and each of those subfolders has 20–30 images that are used for training and testing.
The static folder is divided into the following subfolders: css, js, images, and upload. The css and js directories house the user interface implementation code. Background and display images for web pages can be found in the images and upload subfolders.
Static html web pages in the templates folder are performed based on expected output.
Data collection, data preprocessing, cnn model building and training, and prediction are all modules included in this project.
The dataset contains images with several diseases in tomato plants. Some of the images areextracted from the internet and some are captured from the farm using a camera device.

## TRAINING.PY
Tensorflow and Keras libraries, among others, are first imported.Layers like convolutional, pooling, flattening, and full connected are added once CNN is initialised.
The loaded training and validation sets. Images are read, scaled, and transformed into RGB format with the aid of the CV2 library.With train and valid sets, the classier.fit() method is used to train and validate the model.The model.h5 file is created and stored to the disc after the model has been trained.
In testing modules, this model is loaded and used.

## EXAMPLE.PY
The model that was developed in the prior phase is loaded after the appropriate libraries have been imported.One image that has been scaled, turned into an array, and extended in accordance with dimensions is used for testing.Using the value it generates, the model forecasts disease.

## LEAF.PY
Similar to the  functioning of example file , this file Additionally, has capabilities that allow for the dynamic selection of images on web sites, the building of web pages using Flask, and the prediction of disease and its treatment.

## PRACTICAL IMPLEMENTATION OF PROJECT
After training the model, we obtained a 94 percent training accuracy. After training, testing is carried out by running the leaf.py code, which creates a url that must be entered into the web browser. The user interface then appears and prompts us to choose the image. After choosing the image, it makes a diagnosis and suggests a course of treatment.
