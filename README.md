# Data_centric_AI_Contest ( Innovative Submissions Track ) 
Data Centric AI ( MNIST-ROMAN )

1.  "Crop" image first  and then "Augment" provides similar accuracy as "Augmenting" Images first and then "cropping" 
	- Compresses image size by 4x , Facilitates Faster Upload and reduces Colab Workspace
        - Realize Faster image augmentation and DataSet Search easier
        - Achieves similar accuracy to traditional approach 

2.  With Validation dataset unmodified , Discretization of Augmented training dataset improves decision boundary
         - Group pixels of similar intensity to same value
         - Faster convergence with training data , reduces validation loss and improves accuracy with Test Set

3.  Diagonal resets provide better image distoration over random erasing

4.  Emprical results with 
	- Augment all images with its Flip  ( Contrasting Distribution )
	- Mixup 			    ( https://arxiv.org/abs/1710.09412 )

