# Huffman Coding Tree Assignment 

## Introduction 
This exercise demonstrates the creation of a Huffman Coding Tree using Python on Google Colab. The implementation is done according to the steps depicted by the greedy algorithm. It utilizes a tree-building technique through the use of a min-heap. It also solicits user input for character ciphers and their respective frequencies while resolving the situation when two or more characters have the same frequency. In doing so, this it selects the one having automatic priority out of the ones having equal frequencies, which is based on alphabetical order. This program is case insensitive; it means for the program, upper case and lower case are the same. 

The problem features include the following: 

* Min-Heap Data Structure: As the program utilizes Python's heapq library, the it has the efficiency to build the Huffman Tree very quickly.

* Alphabetic Order Progressing: When two or more characters have the same frequency, the program worries about who went first alphabetically.

* Low sensitivity: The program is not sensitive to the case, all the characters will be in lower cases, and the frequencies of the upper case and lower case will be treated as a total.

* User and character input: The program accepts from users, pairs of lower case and upper case characters and their frequencies as input.

* Huffman Codes: After constructing the Huffman Tree, the software program assigns numerical values to the shards making the code tree.

## Instructions 

### 1. User Input:  

Program prompts the user to type in a number of the characters and thereafter each character either in upper or in lower case form and its corresponding frequency. 

### 2. Output:

After processing the input, the program constructs the Huffman Tree and prints the Huffman code for each character.

## Example Input/Output:

### Input:

Enter the number of characters: 4

Enter character: A

Enter frequency: 5

Enter character: B

Enter frequency: 9

Enter character: C

Enter frequency: 12

Enter character: a

Enter frequency: 7


### Output:

Huffman Codes:

b: 00

a: 01

c: 1

In this example, both 'A' and 'a' are treated as the same character due to case insensitivity, and their frequencies are combined. 

## Requirements 

* Python version 3.x 

* Libraries: heapq, collections (both come included with Python) 

## Running the Program in Google Colab 

* Start a new Colab notebook 

* In the notebook copy and paste the already provided code using python programming language. 

* Execute the code and provide necessary inputs required in the form of the characters and their frequencies. 

## Link to Colab Notebook: 

https://colab.research.google.com/drive/1ybYNxNTu3Tb4QZguajlNf7Xy95j7fBIM#scrollTo=Y_fEaPm6gqZG 

## How it Works: 

### 1. Min-Heap Construction: 

The min-heap characterizes that the program extracts always the two smallest frequency characters/nodes. 

The extracted characters are combined into a new node that possesses a frequency value equal to their sum. 

This process is repeated until only one tree is left standing, representing the Huffman Tree.

### 2. Equal frequency:

In cases where two characters were assigned the same frequency, those characters are sorted alphabetically before combining them in the preceding tree.

### 3. Code generation from the Huffman Tree:

To generate binary codes for the characters, the characters’ codes were generated from the last Huffman tree.

## Notes:

The program merges frequencies of upper and lower case characters and treats their occurrences as similar.

When the frequencies are equal, the program ensures the given order.

