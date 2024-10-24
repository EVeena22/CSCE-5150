# Huffman Coding Tree Assignment
## Overview
This project implements a Huffman Coding Tree using Python in Google Colab. The implementation follows a greedy algorithm approach and utilizes a min-heap data structure to construct the tree. Additionally, the program takes user input for characters and their frequencies and handles cases where two or more characters have the same frequency by prioritizing them in alphabetical order. Case sensitivity is ignored, treating uppercase and lowercase characters as the same.

## Features
* Min-Heap Data Structure: Efficiently builds the Huffman Tree using Python's heapq library.
* Alphabetical Ordering: In cases where two or more characters have the same frequency, the program ensures alphabetical order is considered.
* Case Insensitivity: The program treats all characters as lowercase, combining the frequencies of uppercase and lowercase letters.
* User Input: The user can input pairs of characters (both uppercase and lowercase) and their corresponding frequencies.
* Huffman Codes: After constructing the Huffman Tree, the program outputs the Huffman code for each character.
## Instructions
### 1. User Input:

The program prompts the user to input the number of characters, then each character (as either upper or lowercase) and its frequency.
All characters are automatically treated as lowercase.
### 2. Output:

After processing the input, the program constructs the Huffman Tree and prints the Huffman code for each character.

## Example Input/Output:

### Input:

Enter the number of characters: 4

Enter character: a

Enter frequency: 6

Enter character: b

Enter frequency: 14

Enter character: c

Enter frequency: 12

Enter character: d

Enter frequency: 28

### Output:

Huffman Codes:

d: 0

b: 10

a: 110

c: 111

## Requirements
* Python version 3.x
* Libraries: heapq, collections (both are part of Python's standard library)
  
## Running the Program in Google Colab
* Open a new Colab notebook.
* Copy and paste the provided Python code into the notebook.
* Run the code, and follow the instructions for entering characters and their frequencies.
  
## Link to Colab Notebook:
https://colab.research.google.com/drive/1ybYNxNTu3Tb4QZguajlNf7Xy95j7fBIM#scrollTo=Y_fEaPm6gqZG

## How it Works:
### 1. Min-Heap Construction:

The program uses a min-heap to always extract the two smallest frequency characters/nodes.
The extracted characters are combined into a new node with a frequency equal to their sum.
This process repeats until a single tree remains, which represents the Huffman Tree.
### 2. Handling Equal Frequencies:

If two characters have the same frequency, the program sorts them alphabetically before combining them in the tree.

### 3. Huffman Code Generation:

The final Huffman Tree is traversed to generate binary codes for each character.

## Notes:
The program treats upper and lowercase characters as the same and merges their frequencies.
The program guarantees alphabetical ordering when frequencies are equal.
