As the entirety of the Yolov9 model could not be uploaded to GitHub, I have uploaded the dataset and code that I primarily utilised during my experimentation to the project. 

If you have any queries pertaining to Yolov9, please contact:22hylin@stu.edu.cn. 

If I receive the email you sent, I will endeavour to assist you with any queries you may have regarding the Yolov9 model process.

The following section will present the current graph of the application of Yolov9 to fish fry identification and counting, as well as a graph of the optimal prediction results:

1.Pictures of fish fry to be predicted:

a)
<img src="https://github.com/WEllin06/Yolov9-In-Specific-Practice/assets/131169223/3c2ea146-bed4-4d84-a22f-1d87f4b87ab2" width="300px">

b)
<img src="https://github.com/WEllin06/Yolov9-In-Specific-Practice/assets/131169223/16e9ac4e-faa3-44d4-a3c2-9600bd5726f1" width="300px">

c)
<img src="https://github.com/WEllin06/Yolov9-In-Specific-Practice/assets/131169223/2d188eaa-935b-4c8b-a451-e88277a97dc6" width="300px">

2.Fish fry identification results:

a)
<img src="https://github.com/WEllin06/Yolov9-In-Specific-Practice/assets/131169223/be67d3fd-4bda-4d99-ab48-2ea8587bbf85" width="300px">

b)
<img src="https://github.com/WEllin06/Yolov9-In-Specific-Practice/assets/131169223/c6ba771a-1691-41d0-8f65-f609176c8fae" width="300px">

c)
<img src="https://github.com/WEllin06/Yolov9-In-Specific-Practice/assets/131169223/1554536a-4710-4d4f-8bfc-fe25b08cb783" width="300px">

Analysis of experimental results:

Although the predicted number of fish fry is the same as the actual number of fish fry, after careful observation of the prediction result graph, this paper found that: this is because there is a certain fish fry was repeatedly predicted and counted in the prediction result (increase) or multiple fish fry overlapped and were predicted as one fish fry (decrease), so that the overall prediction result (increase+decrease=equilibrium) is the same as the actual result. This is a problem worth pondering over, and if the nature of the problem is analysed, only then it is possible to make further improvements in the various metrics of the model. And this study believes that pre-processing the image, such as: adding greyscaling,, binarization, filtering, expansion, erosion and other operations before inputting the model for training may be able to mitigate the influence of colour, shape and other features on the model error.

