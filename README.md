# CIFAR100_with_KERAS
CNN over CIFAR100 KERAS API Dataset.
Tried Convolutional2D Image Analysis over the dataset to reach a final accuracy of approximately 60% only over the dataset even after 100 epochs that is 100 Back Propogation and 100 Forward Propogation.
So of course this CNN with 'relu' as activation function is not performing too well.
I have tried to visualize how much my model is confident every time with random plots of training data and their following prediction and thus marked as PASSED or FAILED accordingly.
So first of all the problem is - NOT enough dataset wrt to the number of classes/fine_labels i.e. 100 in CIFAR100.
I hope someone coming to this use case after solving CIFAR10 Project only. If not please kindly warm up with the CIFAR10 dataset then only you will understand why the same procedure was giving quite good output on CIFAR10 and not on CIFAR100.
In both CIFAR100 and CIFAR10 dataset the number of training images are 50000 and testing is 10000 but still accuracy is different in both. The main reason is insufficient data. If you can find the unique number and count of images per label in y_train you will find for every fine label there is only 500 images. And there are 100 labels. So total 500(images per fine_label)*100(fine_labels) = 50,000 images only.
But in CIFAR10 5000(images per label)*10(labels) = 50,000 images only.
That creates the difference. Insufficient data for CNN will lead to low accuracy for sure.

Updated the code with real life and recent google images of 10 different catagories and the changed their pixel one by one and then let the model predict the output.
which seems that the model is not so much accurate as it was showing before for the inbuilt 10000 testing image datasets only.
6 failed out of 10 clear images uploaded and crossverified. So accuracy in real life lowers down to around 40% from 60% achieved on inbuilt data which shows kind of biased dataset wrt to recent images bcz those training images were really very old datasets wrt to images I used for the cross verification.
