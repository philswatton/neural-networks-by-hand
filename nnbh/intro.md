# Neural Networks by Hand

WIP

In this [jupyter book](https://jupyterbook.org/en/stable/intro.html), I set out how to build a feedforward neural network function from scratch using only base python and numpy. Before doing that, I cover most of the pre-requisite math for deep learning, including matrix algebra, vector caclulus, and gradient descent.

## About the notebook

This notebook largely exists for the purpose of my own self-learning. In that light, it's mostly a document of my own notes from many sources, synthesised and repeated for the sake of developing my understanding. There isn't anything original here in terms of *content*, but there may be in terms of the specific combination and presentation of that content (though probably not!).

I'm putting it online for three reasons. First, so I can easily refer back to it later. Second, to show that I am sufficiently familiar with the substance of deep learning to write a document like this. Third, because it will hopefully help someone else on their own learning journey.

One thing that's a little different about the python code presented at the end of this Jupyter book is that many other neural network by hand type tutorials I've encountered typically focus on neural networks with either a single or at most two hidden layers, or don't present (all of the) equations in matrix form. I personally benefit a lot from underestanding general solutions and implementations, so that's what I've tried to do here. In practice, this means that I set out to write a neural network function that:

- allows an arbitrary number of hidden layers
- allows arbitrary width of each hidden layer
- with different activation functions available both for hidden and output layers
- with different loss functions available

Of course, in practice the one thing I won't be doing is writing super-optimised code. So 'arbitary' depth and width will have some the natural contrains of becoming fairly slow in the time it takes for something to be computed (as compared to implementations such as those in e.g. well-established Python libraries).

I've borrowed extensively from several courses, documents, textbooks, stackexchange answers and wikipedia articles in the course of putting these notes together. As with other things, I found that re-reading the same thing in different ways helped me to better understand it. My background prior to my current position as a data scientist was in political science, where there was much more emphasis on statistics than machine learning. So, if that's also your background, then hopefully this list of resources to which this jupyter book owes a lot will help you on your own learning journey:

## Some further readings

Before reading the pages here, it's worth considering the resources I learned from in order to be able to put all of this together. In many cases these are probably better resoruces than the one here, and so you're likely to get more benefit out of them than you are out of using this document.

Before getting into deep learning, it's worth familiarising yourself with machine learning more broadly. I'd recommend these two resources:

- Statistical modeling: The two cultures by Leo Breiman (a classic), [link](https://projecteuclid.org/journals/statistical-science/volume-16/issue-3/Statistical-Modeling--The-Two-Cultures-with-comments-and-a/10.1214/ss/1009213726.full)
- Machine Learning for the Social Sciences, an Agnostic Approach by Justin Grimmer, Margret Roberts, and Brandon Stewart (a must-read for social scientists coming at this from a stats background), [link](https://www.annualreviews.org/doi/abs/10.1146/annurev-polisci-053119-015921)

Once you've got those under your belt, I'd recommend starting with the following paper. It's a summary of deep learning for psychologists, but it's a great read for any social scientist looking to familiarise themselves with deep learning:

- Deep learning: A primer for psychologists by Christopher Urban and Kathleen Gates, [link](https://psycnet.apa.org/record/2021-31499-001)

Once you've read that, the main resources I used in being able to build this jupyter book (although this list should not be taken as exhaustive - there were of course many stackexchange posts and other similarly helpful webpages on the way):

- Machine Learning Specialisation by Andrew Ng, [link](https://www.coursera.org/specializations/machine-learning-introduction)
- Deep Learning Specialisation by Andrew Ng, [link](https://www.coursera.org/specializations/deep-learning)
- The Matrix Calculus You Need For Deep Learning by Terrence Parr and Jeremy Howard, [link](https://explained.ai/matrix-calculus/), [paper version](https://arxiv.org/abs/1802.01528)
- Neural Networks and Deep Learning by Michael Nielsen, [link](http://neuralnetworksanddeeplearning.com/index.html)
- Sten Stootla's blog
  - [On backprop](https://sootlasten.github.io/2016/gd-backprop-derivation/)
  - [On backprop with softmax](https://sootlasten.github.io/2016/softmax-backprop-derivation/)

In particular I found *The Matrix Calculus You Need For Deep Learning* incredibly helpful for wrapping my haid around the vector/matrix calculus used in estimating the neural networks. It's a document I'd recommend to anyone trying to wrap their head around backpropagation in particular. Michael Nielsen's *Neural Networks and Deep Learning* was likewise the moment backpropagation finally clicked for me, and I throughly recommend it as well.
