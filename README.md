# Data_centric_AI_Contest ( Innovative Submissions Track ) 
We describe 4 innovative approaches towards Data Centric AI ( MNIST-ROMAN )

1.  "Crop" image first  and then "Augment" provides similar accuracy as "Augmenting" Images first and then "cropping" 
	- Compresses image size by 4-16x , Facilitates Faster Upload and reduces Colab Workspace
        - Realize Faster image augmentation and Simplifies DataSet Search
        - Achieves similar accuracy as that of traditional approach 

Cropped Image 


![ab9fb784-ce5d-11eb-b317-38f9d35ea60f](https://user-images.githubusercontent.com/4832280/129690470-cebdaf92-3546-4754-9051-3f1cde973a03.png)

Original Image

![ab9fb784-ce5d-11eb-b317-38f9d35ea60f](https://user-images.githubusercontent.com/4832280/129689863-64dd57f1-2c53-4d0f-82a6-99d551fe6960.png)

2.  With Validation dataset unmodified , Discretization of Augmented training dataset improves decision boundary

         - Group pixels of similar intensity to same value
         - Faster convergence with training data 
         - Reduces validation loss and emprical results suggest improved accuracy with Test Set

3.  Diagonal Resets could better distort HandWritten Images over Random Erasing 

4.  Emprical results with 
	- Augment all images with its Flip  ( Contrasting Distribution )
	- Mixup 			    ( https://arxiv.org/abs/1710.09412 )

