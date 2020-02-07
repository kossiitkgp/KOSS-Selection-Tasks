# Story
Categorial Data(data type is not a number like name of state, day or gender) cannot be fed directly into few Machine Learning Models. They are converted into numerical data using different encoding algorithm. One simplest among them is one hot encoding.

# Materials
- https://machinelearningmastery.com/why-one-hot-encode-data-in-machine-learning/

# What you need to do
- A csv will be given to you, you need to apply one hot encoding algorithm from scratch in python make another csv file. You should neither use pandas' getdummiers and Categorial nor sklearn library. 
Example : 
| Name          | Favourite Color   | 
| ------------- |:-------------:| 
| Raghav    | red |
| Raja     | blue      |  
| Amar | yellow      |  

| Name          | Favourite Color_red   | Favourite Color_blue   | Favourite Color_yellow   | 
| ------------- |:-------------:| 
| Raghav    | 1 | 0 |0 |
| Raja     | 0      | 1      |0      | 
| Amar | 0      |  0 | 1|

# Tech Stack
Use python and its csv library to handle the csv file. You are free to convert it into a pandas  dataframe and play with it. PLEASE DO NOT USE getdummies to hot encode of pandas. However you are free to use other pandas features.

# Learning from the task
You will learn to handle a csv file in a programmer's way(which we do on a regular basis) for different purposes like sending mails and will also improve your googling skills. We encourage you to use pandas(not its getdummies API) and to realize how powerful it is. 