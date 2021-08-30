# Data_centric_AI_Contest 
Interesting approaches towards Data Centric AI contest ( MNIST-ROMAN )

1.  "Crop" image first  and then "Augment" provides similar accuracy as "Augmenting" Images first and then "cropping"  with benifits in space and faster Augmentation

     10X compression in DataSet size

	![image](https://user-images.githubusercontent.com/4832280/131283487-3a891061-6175-471b-9ac3-2122bed56db4.png)
  
        ![image](https://user-images.githubusercontent.com/4832280/131283548-187a0e0f-885e-440b-b050-5c6a1bb6c86d.png)



2.  We also observe the follow Approaches to help tweak training data distribution and improving validation accuracy  
      
         - Group pixels of similar intensity to same value ( Group by a factor of 2 or 3 works well to several of training datasets and
           reduces variance . However a large Group factor increases bias )
         - Random shift ( increasing low intensity pixels while decrease high intensity pixels with random value appears to be a useful
           way to modify data distribution in several cases than scaling image by a constant factor that converts high intensity to low
           intensity because of overflow)
         - Diagonal resets appear to better distort handwritten text over random erasing
         
         


