The assignment consists on 3 different files names Facial_Recognition_project.Rmd, Final_ModelPCA.Rdata and Final_ModelFisher.Rdata. We will now explain what each of them are and how they are supposed to be used.


- Facial_Recognition_project.Rmd: An Rmarkdown report containing the code and explanation followed when carrying out the training. It runs from start to end without the need for any extra steps. It is the main body of the assignment.


- Final_ModelPCA.Rdata: This file contains the final model and the classifier built using PCA. The model consists on a few R objects (as detailed in the report) and a classifier function called Facial_Recognition. It also includes an auxiliary function the classifier calls to when used. To use this it is necessary to load these objects into R using the following command:
	
				load("Final_ModelPCA.Rdata")

Once executed, all files will be loaded into the workspace. To use the classifier, the following R function must be called with an image "Image.jpg" as its argument. The classifier only works for images of size 200x180 (otherwise it returns an error).

				Facial_Recognition("Image.jpg")


- Final_ModelFisher.Rdata: This file contains the final model and the classifier built using Fisher discriminant analysis. The model consists on a few R objects (as detailed in the report) and a classifier function called Facial_Recognition_fisher. It also includes an auxiliary function the classifier calls to when used. To use this it is necessary to load these objects into R using the following command:
	
				load("Final_ModelFisher.Rdata")

Once executed, all files will be loaded into the workspace. To use the classifier, the following R function must be called with an image "Image.jpg" as its argument. The classifier only works for images of size 200x180 (otherwise it returns an error).

				Facial_Recognition_fisher("Image.jpg")
