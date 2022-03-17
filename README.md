<h1> Forever an Author - a Recurrent Neural Network with a Long-Short Term Model </h1>

<h2> Overview </h2>

Seminal authors and poets are often championed for their works only after their passings, leaving open the possibility of "what wonderful works would they create if only they were alive".
With the use of a simple **Recurrent Neural Network using a Long-Short-Term Model**, this project seaks to answer such a question.

> Using the famed detective novel "The Adventures of Sherlock Holmes" by Sir Arthur Conan Doyle through the open source Gutenberg project, we trained a Recurrent Neural Network, or R.N.N.
to learn and generate texts mimicking the style, structure, and content of the crime fiction thriller. 

<h2> Why R.N.N. </h2>

If you are familiar in working with text generation and text datasets in deep learning applications, you may wonder *why use a R.N.N. instead of another N.L.P. (Natural Language Processor) approach?*
The purpose of an R.N.N. in this context allows the "rememberence" of previous inputs through internal memory, specifically through the **Long-Short-Term Model (L.S.T.M.)**. This will allow us to 
better develop the literary style of the author as opposed to simple generation of text through a more conventional N.L.P.
  
 
<h2> Required Imports </h2>
These include:

- Tensorflow
  >An open-source artificial intelligence library, particularly used for training deep neural networks. We will depend on tensorflow for our optimizer

- Keras
  >An open-source library that provides an interfaces for our tensorflow based neural networks
  >Keras will provide the layering, activation functions, and optimizers for our R.N.N.

- Numpy
  >A library to support large arrays and functions, which will be required in contorting the book into the appropriate form of information to feed our R.N.N.


<h2> Steps to Building Our Neural Network </h2>

1. Loading in the data
  > Importing the data in the right manner is crucial first step to effectively achieving our goal. In this project, we import the book through the **Gutenberg eBook Online Library**, an open sourced collection of books. 
  > The website can be found [here](https://www.gutenberg.org/files/1661/1661-0.txt)

2. Changing our Data
  > Next step is to change our character mapping from characters to integers into integers to characters, which will allow the dataset better processing by the computer.

3. Splitting our Integers
  > After, we split our sequences of characters into 3 separate fragments in *arrays* with 40 character sequences at each index of our arrays. 

4. Changing our Data Type
  > Further, we change our array of character sequences into a boolean array for the computer to comprehend

5. Build the R.N.N.
  > At this point, our data is prepped, so we can proceed with building our R.N.N., calling on in built layering through the **Keras library** to create a sequential model
  > with a **L.S.T.M.** model, a dense layer, a **softmax** activation function, and a **RMSProp** optimizer with specified hyperparameters. 

6. Helper Functions
  > These are used to improve our model as it trains

7. Callback Functions
  > To help imrpove our learning rate across multiple epochs, we create callback functions, similar to "checkpoints" for our R.N.N. to build off of and reduce our learning rate loss


<h2> Training and Testing </h2>

To train our model, we simply fit it to our specified parameters with the appropriate functions and generate texts using a function with parameters of length and diversity, which was created 
as an add-in for *style*, mimicking more verbose vernacular and looser sentence structure associated with the literature and language of the time.

<h2> Results </h2> 



<h2> Conclusion </h2>


<h2> Resources </h2>

Text data found (here)[https://www.gutenberg.org/files/1661/1661-0.txt]

Jupyter Notebook found (here)[]

Medium Article found (here)[]


