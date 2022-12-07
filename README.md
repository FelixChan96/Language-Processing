# Language Processing Sample Work 

Please read the description below before checking out the report PDFs as well as the Python scripts.

**Description of tasks**

Implementing a Pytorch program that learns to read business reviews in text format and predict a rating (positive or negative) associated with each review, as well as a business category (0=Restaurants, 1=Shopping, 2=Home Services, 3=Health & Medical, 4=Automotive). 

Please read the description below before checking out the report PDFs as well as the Python scripts.

The report outlines how my program works and explains design decisions.

How I selected your architecture, algorithms, and enhancements. How I chose your cost function and optimiser. How I determined the dimensionality of the word vectors, metaparameter values, and any data preprocessing that I did or did not use. How I employed the validation set, and any additional steps to avoid overfitting not otherwise discussed. My task was to complete the file student.py in such a way that it can be run in conjunction with a3main.py by typing:

python3 a3main.py

The provided file a3main.py handles the following:

(**Directions from the assignment**): Loading the data from train.json Splitting the data into training and validation sets (in the ratio specified by trainValSplit) Data Processing: strings are converted to lower case, and lengths of the reviews are calculated and added to the dataset (this allows for dynamic padding). You can optionally add your own preprocessing, postprocessing and stop_words (Note that none of this is necessarily required, but it is possible). Vectorization, using torchtext GloVe vectors 6B. Batching, using the BucketIterator() provided by torchtext so as to batch together reviews of similar length. This is not necessary for accuracy but will speed up training since the total sequence length can be reduced for some batches. You should aim to keep your code backend-agnostic in the sense that it can run on either a CPU or GPU. This is generally achieved using the .to(device) function. If you do not have access to a GPU, you should at least ensure that your code runs correctly on a CPU.
