# hw1. generate PAM<sub>x</sub> matrix
* your name
* student ID

## Description

* Writing Python program to generate PAM<sub>x</sub> from the given mutation probability matrix.
* PAM<sub>x</sub> must be as a log odds and complete square matrix (rounding to integer), not the format of the given mutation probability matrix.
* Creating your own program, i.e., hw1.py, to read mut.txt and *x*, then output pamx.txt.

* You need to write your program as a function named generate_pam. i.e.,
```
def generate_pam(x, input_path, output_path):
    .
    .
    .
    .
```
* Upload your code 'hw1.py' to Gradescope under the course ID:**8K4V8V**.
* Packages you can use: numpy, pandas

### HINTs
* PAM<sub>x</sub> is a symmetric matrix even though the given mutation probability matrix is not.
* The mutation matrix should be divided by 10,000 before calculation PAM250. The value in the matrix should be in [0,1].
* Normalized frequencies of amino acids (<I>f<sub>i</sub></I>) credit by [Bioinformatics and Functional Genomics 3rd edition](https://www.wiley.com/en-us/Bioinformatics+and+Functional+Genomics,+3rd+Edition-p-9781118581780) 
![image](frequent.png)

## Parameters

* x: parameter of pam
* input_path: input file path
* output_path: output file path


## Files

* mut.txt: the input mutation probability matrix, M<sub>1</sub>
* pam250.txt: the output generated by generate_pam(250, 'example/mut.txt', 'example/pam250.txt'). The output format must be identical to the one of pam250.txt.


## Evaluation

There are 10 testing data (5 public, 5 private). 
* Correct answer gets 10 points for each testing data.


### Penalty

* If your code is similar to others and lacks detailed comments, you may lose up to 10 points or possibly receive a zero.

## References
Please provide the code along with its reference. For example, you can cite it as: ```# ChatGPT, respond to “your prompt,” on February 16, 2023```. Below is an example of a reference format summarizing the use of ChatGPT for R programming

>You are the R Language expert.
>Please help me to write a function call “k_fold” .
>Using given dataset to train the random forest model, and use the k-fold cross- validation to evaluate the best model parameters. Here is the instruction of the function requirements:\
>Function name: k_fold\
>Function parameters:
>1. k: the number of how much fold to split the dataset doing the k-fold cross- validation.
>2. input_file: input csv file path.
>3. output_file: output path of k-fold cross-validation result.
