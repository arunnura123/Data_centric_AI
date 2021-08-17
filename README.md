# Data_centric_AI_Contest
Data Centric AI

1.  Crop image first  and then Augment provides similar accuracy as Augmenting first and then cropping 
	- Compresses image size by 4x , Facilitates Faster Upload and reduces Colab Workspace
        - Realize Faster image augmentation and DataSet Search easier
        - Achieves similar accuracy to traditional approach 

2.  With Validation set unmodified , Discretization of training dataset improves decision boundary
         - Group pixels of similar intensity to same value
         - Faster convergence with training data , improved loss with validation set and accuracy with Test Set

3.  Diagonal resets provide better image distoration over random erasing

