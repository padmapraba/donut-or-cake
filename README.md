# donut-or-cake
Image classifier that predicts if an image is a doughnut or a chocolate cake

For this implemenntation of an Image Classifier the Keras API was used to implemennt the the deep learning models.
The data set of images were obtained from a public dataset on Kaggle. 1000 images of donuts and chocolate cake was used with a 80-20 split.
The data was also augmented to compensate for the small amount of data used.
The method of transfer learning and fine-tuning was used to save time. The model was built using weights pre-trained on a xception CNN architecture.
This base model was frozen and a new model was created onn top.
The input was then normalized as it is a requirement to using pre-trained Xception weights.
The top layer was then trained and then tested with random images.

Bibliography:

  https://keras.io/examples/vision/image_classification_from_scratch/
  
  https://keras.io/guides/transfer_learning/#an-endtoend-example-finetuning-an-image-classification-model-on-a-cats-vs-dogs-dataset
  
  https://www.kaggle.com/kmader/food41
