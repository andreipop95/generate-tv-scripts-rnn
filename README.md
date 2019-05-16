# Generate TV Scripts
Generate fake TV scripts inspired from previous scripts using RNNs 

This project has been done as a part of the [Udacity Deep Learning Nanodegree](https://eu.udacity.com/course/deep-learning-nanodegree--nd101)

## Project's objective
The objective of this project is to generate a fake TV script by using a known dataset called Seinfield. The generated script is based on the patterns that the RNN recognizes in the data.

## About the RNN's architecture
**Embedding Layer** - this layer has been used for dimensionality reduction. Another possbile approach would have been one hot encoding. Since there are a few thousands of words, this is not feasible.
<br/>
**LSTM layer** - these layers add recurrent connections to the network and give the possiblity to include information about a sequence of words
<br/>
**Linear layer** - this layer will output the data in the desired dimensions
<br/>

## Resources used

[Seinfield dataset](https://www.kaggle.com/thec03u5/seinfeld-chronicles#scripts.csv)

## Results obtained
The text below has been obtained after training the network. It doesn't really make sense, but there are a few patterns that can be observed:

jerry: the law. <br/>
jerry: oh, no, no. no. it's not a good thing, and you were in the middle of a little playworld- shirt? <br/>
george: i can't get it! <br/>
kramer: oh, i got it. <br/>
hoyt: you know what? the whole thing is robbing robbing. <br/>
george: well, this is my grandson. <br/>

## How to run the current project

The prerequisites in order to set the project on a local machine are:
* [Github](https://gist.github.com/derhuerst/1b15ff4652a867391f03)
* [Anaconda and python](https://docs.conda.io/projects/conda/en/latest/user-guide/install/windows.html)

1. Git clone the repository
   
   `git clone https://github.com/andreipop95/generate_tv_scripts.git`

2. Create a conda environment using python 3.5. As an alternative for package management, pip can be used

   `conda create --name <your_project_name> python=3.5`
   `source activate <your_project_name>`

3. Install needed packages
   
   `conda install <package_name_1 package_name_2...>`
   
4. Install jupyter notebook
   
   `conda install jupyter notebook`
 
5. Lunch the notebook
   
   `jupyter notebook dlnd_tv_script_generation.ipynb`
