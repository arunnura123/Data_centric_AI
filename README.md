# Data_centric_AI_Contest 
Interesting approaches towards Data Centric AI  ( MNIST-ROMAN )

1.  Resize as an augmentation technique not only reduces image size in disk but reduces variance . 
    Resize less than 8*8 leads to accuracy degrade - Random resize between 16*16 to 32*32 works better 

        - 10X compression in DataSet size
        - Faster Augmentation with commodity devices
        - Avoids preprocessing overhead during training time
        - Improves Ease of Dataset Manipulations ( Fixing Datasets ) 

	![image](https://user-images.githubusercontent.com/4832280/131283487-3a891061-6175-471b-9ac3-2122bed56db4.png)
	
      Original Image Size 
  
     ![Original](https://user-images.githubusercontent.com/4832280/131283812-470058c7-90ff-46f9-ba3b-665aa994f694.PNG)


2.  Other Interesting Approaches to Augment Images 
      
         - Binning / Discretization 
       
                - Linear Mapping  - Group pixels of similar intensity to same value ( Group by a factor of 2 or 3 works well to 
           several of training datasets and experiments show reduction in variance . However a large Group factor degrades performance )
	   
	 		- Non Linear Mapping - Quantized Pixel values are mapped with non linear scale
	   
         - Random shift
                Increasing low intensity pixels while decrease high intensity pixels with random factor appears to be a useful
           way to modify data distribution in several cases 
	   
         - Clip First and then Scale 
                Scaling image by scale factor results in overflow ( 255 ) resulting in poor Augmentation. Instead Clip by threshold or 
	  	 value and then scale by 255/threshold as scale factor increases magnitude of low intensity pixels ( better Augmentation )
		 
		 
3.  Observations 

      - A combination of these techniques appear to  result in better augmentation ( by varying distribution ) of training data  


     Variations of cropped Images with Binning , Random Shift and "Clip First and then Scale" 

![image](https://user-images.githubusercontent.com/4832280/131782644-05918ccf-f426-4b07-b137-bfee92d0e299.png)

4.   Challenges with Augmentation

	 Zoom - 8 is not clearly recognizable

![image](https://user-images.githubusercontent.com/4832280/131782872-9daebe29-4292-4ed8-8bd9-6df1fb2a6b45.png)

	 Scaling Image leading to significant change in distribution ( Addressed by Clip first and scale )

![scale_processedac21d4d0-ce5d-11eb-b317-38f9d35ea60f](https://user-images.githubusercontent.com/4832280/131783752-adbce163-7265-4da0-bffb-1759b208613d.png)



   
