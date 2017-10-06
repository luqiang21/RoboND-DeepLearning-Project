
# 1.The write-up conveys the an understanding of the network architecture.

| layers        | dimension           | filter  |
| ------------- |:-------------:| -----:|
| encoder 1 | 

The student clearly explains each layer of the network architecture and the role that it plays in the overall network. The student can demonstrate the benefits and/or drawbacks different network architectures pertaining to this project and can justify the current network with factual data. Any choice of configurable parameters should also be explained in the network architecture.

The student shall also provide a graph, table, diagram, illustration or figure for the overall network to serve as a reference for the reviewer.

The student should be able to clearly explain the purpose of each layer in the network architecture to a reasonable extent. Extreme low-level (granularity) is not required, but a reasonable display of knowledge is required.

# 2. The write-up conveys the student's understanding of the parameters chosen for the the neural network.

The student explains their neural network parameters including the values selected and how these values were obtained (i.e. how was hyper tuning performed? Brute force, etc.) Hyper parameters include, but are not limited to:

Epoch
Learning Rate
Batch Size
Etc.
All configurable parameters should be explicitly stated and justified.

Make sure the student clearly explains each parameter needed. It is important that the student know how hyper tuning this parameters impacts the overall network (and system).

# 3. The student has a clear understanding and is able to identify the use of various techniques and concepts in network layers indicated by the write-up.

The student is demonstrates a clear understanding of 1 by 1 convolutions and where/when/how it should be used.

The student demonstrates a clear understanding of a fully connected layer and where/when/how it should be used.

The student should be able to clearly explain how a 1 by 1 convolution is used, where to use it, and why. The same should also be true for fully-connected layers.

# 4. The student has a clear understanding of image manipulation in the context of the project indicated by the write-up.

The student is able to identify the use of various reasons for encoding / decoding images, when it should be used, why it is useful, and any problems that may arise.

Look to ensure the student knows that encoding images typically removes high frequency data which is not retrievable for it is removed during the decoding stage. In other words, when down sampling an image you are removing high frequency information (i.e. detail). This is because you are removing some of the information from the pixels you removed. To up-sample the best you can do is a slightly worse version than the original if you have no other information about the image.

# 5. The student displays a solid understanding of the limitations to the neural network with the given data chosen for various follow-me scenarios which are conveyed in the write-up.

The student is able to clearly articulate whether this model and data would work well for following another object (dog, cat, car, etc.) instead of a human and if not, what changes would be required.

To successfully satisfy this rubric item the student must address the following issues:

Given the current data is set to follow a person, the data would not work well for following a different object like a car because the system is not trained to do so. The developer would need information on this type of object to train and test to follow a new object.

Model

CRITERIA
MEETS SPECIFICATIONS
REVIEWER TIPS
The model is submitted in the correct format.

The file is in the correct format (.h5) and runs without errors.

The neural network must achieve a minimum level of accuracy for the network implemented.

The neural network should obtain an accuracy greater than or equal to 40% (0.40) using the Intersection over Union (IoU) metric.






Command to upload files to the AWS instance
scp -i "robond.pem" your_file ubuntu@ec2-54-212-223-139.us-west-2.compute.amazonaws.com:~/.

Command to unzip files to a specific folders
unzip file.zip -d your_target_folder
