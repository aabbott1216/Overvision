# Overvision
This project uses computer vision and deep learning to draw bounding boxes around Overwatch heroes. The goal of this project is to accurately draw bounding boxes around Soldier 76 
and be able to train a reinforcement learning agent to track and follow soldier 76. So far Computer vision has been used to draw bounding boxes around many overwatch heroes. See the uploaded images to see the bounding box progress.

This is the first iteration of bounding box training. It is severely underfit:
![image](https://user-images.githubusercontent.com/77586827/114313890-6e51f880-9ac6-11eb-8582-75f6cffab27d.png)

After tweaking and training with 300 positive annotated images and 300 negative images, here are the results:
![image](https://user-images.githubusercontent.com/77586827/114313909-89246d00-9ac6-11eb-8749-8efb6a7fbe7e.png)

The classifier is doing fairly well now. Next steps may be to add a mask to only pickup on red pixels, here is the first trial of applying a red mask filter
![image](https://user-images.githubusercontent.com/77586827/114313951-afe2a380-9ac6-11eb-90fb-c119f2d3c8d9.png)

An outline of Soldier can clearly be seen however the treees in the background also have red pixels along with other items. Tighter pixel values may need to be done.
The classifier works well for other heroes as well
![image](https://user-images.githubusercontent.com/77586827/114314005-e9b3aa00-9ac6-11eb-8891-aad994ef9e52.png)

But some not so much
![image](https://user-images.githubusercontent.com/77586827/114314010-f89a5c80-9ac6-11eb-92b6-2fb0c33a01d9.png)

I found that the classifier works well with heroes of similar size to soldier

I found this tutorial series to be immensely helpful in the progress so far: https://www.youtube.com/watch?v=XrCAvs9AePM&list=PL1m2M8LQlzfKtkKq2lK5xko4X-8EZzFPI&index=8

I was inspired by this Thesis: https://bit.ly/30EXmn9
