TV Script Generator

RNN TV script generator NLP project for Udacity Deep Learning Nanodegree

Description

Trains an RNN on a dataset of seinfeld screenplays, then generates new, amausing scripts.

# Bike-sharing predictor

#### Returns the expected volume of business based on historical bike-retal data, so the company can predict the number of bikes they will need. First project for the Udacity Deep Learning Nanodegree.

## Getting Started
### Step 1: Review my code in [my_answers.py](https://github.com/technoempathy/bike_sharing/blob/master/my_answers.py "Title") and see my results in [bike_sharing.ipynb](https://github.com/technoempathy/bike_sharing/blob/master/bike_sharing.ipynb "Title").

### Step 2: Do this project yourself
To make your own Bike-sharing Predictor or review the project specifications, go [here](https://github.com/udacity/deep-learning-v2-pytorch/tree/master/project-bikesharing "Title") and follow the instructions in Udacity's README.

## Prerequisites
1. Jupyter Notebooks
2. GPU
3. The [bike-sharing dataset](https://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset) from the UCI Machine Learning Database. 
4.	Pytorch and Torchvision. For installation instructions see [Udacity's README in the Deep Learning repository](https://github.com/udacity/deep-learning-v2-pytorch "Title").

## Tips
#### Watch out for size mismatch. 
Almost all the challenges I ran into with this project happened as a result of size mismatch. Read the comments in my code to see where I had these problems and how I solved them.

## Known Issues
To pass all unit tests, I needed to add this print statement to the test_run function under unittests.
`print(network.run(inputs))`

The print statment should be added here:
```
def test_run(self):
        # Test correctness of run method
        network = NeuralNetwork(3, 2, 1, 0.5)
        network.weights_input_to_hidden = test_w_i_h.copy()
        network.weights_hidden_to_output = test_w_h_o.copy()
        print(network.run(inputs)) #Add the print statement here
        self.assertTrue(np.allclose(network.run(inputs), 0.09998924))
 ```

## Authors
- @technoempathy – Layla Messner 

## Acknowledgments
-	@udacity for the project
-	@facebook for the scholarship to the Udacity Deep Learning Nanodegree
