# Head_pose-Estimation

          

[![Watch the video](https://youtu.be/OKc0SQY3cuI )

                                    

           
Head pose estimation means find (yaw, pitch, roll) angeles of head during motion.

- In this project i worked on **AFLW2000** dataset that contains traing images. Each image has two format (.jpg and .mat).
- **.mat** files contains meta data about corresponds **.jpg**, such as:
    1.  68-face-landmarks, each point represented by (x,y). 
          ![image](https://user-images.githubusercontent.com/53664496/174450652-52ac6957-1c75-40a4-bc2b-7d9a9463bc60.png)

    3.  pose which contains  (yaw, pitch, roll) for that image,
          ![image](https://user-images.githubusercontent.com/53664496/174450676-8bdb5bda-41d1-4442-a0bd-49868460df3f.png)

    5.  and many other meta data.




- I did not work on 68 point for land marks in **.mat** file, But I used **mediapipe** library to extract face-mesh which is 468 point.
      ![image](https://user-images.githubusercontent.com/53664496/174450753-98093d84-9896-4ee6-bd04-3f3ee2e86818.png)
      
- For modeling I used:
    1.  **MultiLinearReagressor** but r2_score is very bad.
    2.  **GridSearch** with **XGBoostRegressor** to find best estimator,  and result was good.
 -Used Library:
  1.  **mediapipe**
  2.  **Dlib**.
  3.  **MultiLinearReagressor**
  4.  **GridSearch**
  5.  **XGBoostRegressor**
  6.  **pandas**
  7.  **numpy**
  

https://user-images.githubusercontent.com/53664496/174451171-752ab062-d378-4260-b17a-b7c2c7f1185d.mp4





