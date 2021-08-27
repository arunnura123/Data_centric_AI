# Data_centric_AI_Contest 
We describe interesting approaches towards Data Centric AI contest ( MNIST-ROMAN )

1.  "Crop" image first  and then "Augment" provides similar accuracy as "Augmenting" Images first and then "cropping"  with benifits in space and faster Augmentation

	- Compresses image size by 4-16x , Facilitates Faster Upload and reduces Colab Workspace
        - Realize Faster image augmentation 
        - Simplifies DataSet correction as image sizes are small
        - Achieves similar accuracy as that of traditional approach 


2.  We also observe the follow Approaches to help tweak training data distribution and improving validation accuracy  
      
         - Group pixels of similar intensity to same value ( Group by a factor of 2 or 3 works well to several of training datasets and
           reduces variance . However a large Group factor increases bias )
         - Random shift ( increasing low intensity pixels while decrease high intensity pixels with random value appears to fare well in several cases
           than scaling image by a constant factor )
         - Diagonal resets appear to better distort handwritten text over random erasing
         
         


