# AIM: Implement and demonstrate the FIND-S algorithm for finding the most
specific hypothesis based on a given set of training data samples. Read the
training data from a .CSV file.

## Theory:

In order to understand Find S algorithm,the understanding of following concepts is needed:
Concept learning
Specific hypothesis
General hypothesis

Concept learning:
The special features differentiate the set of cars, trucks, etc from the larger set of vehicles. These features that define the set of cars, trucks, etc are known as concepts.
Machines can also learn from concepts to identify whether an object belongs to a particular category or not.
Any algorithm that supports concept learning requires the following:
Training data
Target concept
Actual Data Objects

      b.  General hypothesis:
States general relationship between major attributes
G={‘?’, ‘?’ , ‘?’ , ‘?’ ,‘?’ }

	      c.  Specific Hypothesis:
. The specific hypothesis deals with important details about the variables given in the general hypothesis.
S = {‘Φ’,’Φ’,’Φ’, ……,’Φ’}

	## 2. Find S Algorithm:
Initialize ‘h’ to the most specific hypothesis
The find s algorithms considers only the positive examples and eliminates negative examples
For each positive value, the algo checks for the each attribute in the example
If the attribute value is same as hypothesis value, do nothing
Else,if the attribute value is not the same as hypothesis value, the algorithm changes to “?”



## 3. Limitations of Find-S Algorithm
There are a few limitations of the Find-S algorithm listed down below:
There is no way to determine if the hypothesis is consistent throughout the data.
Inconsistent training sets can actually mislead the Find-S algorithm, since it ignores the negative examples.
The Find-S algorithm does not provide a backtracking technique to determine the best possible changes that could be done to improve the resulting hypothesis.

## 4. IMPLEMENTATION OF FIND S ALGORITHM
The concept of this particular problem will be on what days does a person likes to go on walk.


Looking at the data set, we have six attributes and a final attribute that defines the positive or negative example. In this case, yes is a positive example, which means the person will go for a walk.
So now, the general hypothesis is:
h0 = {‘Morning’, ‘Sunny’, ‘Warm’, ‘Yes’, ‘Mild’, ‘Strong’}
This is our general hypothesis, and now we will consider each example one by one, but only the positive examples.
h1= {‘Morning’, ‘Sunny’, ‘?’, ‘Yes’, ‘?’, ‘?’}
h2 = {‘?’, ‘Sunny’, ‘?’, ‘Yes’, ‘?’, ‘?’}
We replaced all the different values in the general hypothesis to get a resultant hypothesis.

# Output
![image](https://user-images.githubusercontent.com/84711076/216431743-9ed48945-0891-4825-811f-18bd1c6d9fd3.png)

Reference : [edureka.co]( https://www.edureka.co/blog/find-s-algorithm-in-machine-learning/)
