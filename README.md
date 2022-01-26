# Auto Annotator
YOLO auto annotator

Consider you have a dataset of animals, and your dataset only has one label (0: animal), but you want a more specific dataset, which is labeld by the name of each animal (0:dog, 1: cat, 2: horse, ...).  
There are two ways to create such dataset:  
1. Label the object (animals) manually
Good Luck!
3. Label them automatically with the help of a classifier  
So if you choose the second option you need to train a classifier to classifies the animals and then use this classifier to label the objects.  
In order to do that we crop the bounding box from the image (which is an animal) and feed it to our classifier.  
After we fed our object to the classifier and the classifier, classified it for us (labeled it), we use the label for our annotation and save it in YOLO format.
