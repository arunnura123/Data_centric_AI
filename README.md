# Data_centric_AI_Contest ( Innovative Submissions Track ) 
We describe 4 innovative approaches towards Data Centric AI contest ( MNIST-ROMAN )

1.  "Crop" image first  and then "Augment" provides similar accuracy as "Augmenting" Images first and then "cropping" 
	- Compresses image size by 4-16x , Facilitates Faster Upload and reduces Colab Workspace
        - Realize Faster image augmentation and Simplifies DataSet Search
        - Achieves similar accuracy as that of traditional approach 


2.  With Validation dataset unmodified , Discretization of Augmented training dataset improves decision boundary

         - Group pixels of similar intensity to same value
         - Faster convergence with training data 
         - Reduces validation loss and emprical results suggest improved accuracy with Test Set

3.  Distort HandWritten Images with Diagonal Erasing 

4.  Emprical results with 
	- Contrasting Distribution          ( Augment every image with a Flip )
	- Mixup 			    ( https://arxiv.org/abs/1710.09412 )

