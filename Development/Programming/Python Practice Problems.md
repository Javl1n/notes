# Beginner Problems
## String Reversal with Vowels
### Description
Write a program that reverses a string while keeping the vowels in their original positions.
### Solution
```
n = int(input(""))
test_cases = [''] * n
for i in range(n):
    test_cases[i] = input('')

vowels = ['a', 'e', 'i', 'o', 'u']

print("\nResults:")

for case in test_cases:
    consonants = ''
    # get all consonants
    for letter in case:
        if not letter.lower() in vowels:
            consonants += letter
    
    # reverse consonant string
    consonants = consonants[::-1]
    
    # initialize string
    string = ''
    
    # put the reversed consonants plus the vowels
    for index2, letter2 in enumerate(case):
        if not letter2.lower() in vowels:
            string += consonants[0]
            consonants = consonants[1:]
        else:
            string += letter2
    
    print(string)
```

## Number Palindrome Checker
**Description**: Write a program that checks if a given number is a palindrome. A palindrome reads the same forwards and backwards.
**Time of Completion**: 3:53 pm - 3:58 pm (5 minutes)
### Solution
```
n = int(input(""))

test_cases = [""] * n

for i in range(n):
    test_cases[i] = input("")

print("Results: ")

for test_case in test_cases:
    print("YES" if (test_case == test_case[::-1]) else "NO")
```

# Easy Problems
## Binary Tree Level Order Traversal
**Description**: Given a binary tree, implement a function to perform level-order traversal and return the nodes at each level as a list of lists.
**Time of Completion**: 48 min.
### Solution
```
# Online Python compiler (interpreter) to run Python online.
# Write Python 3 code in this online editor and run it

n = int(input("Enter n: "))

inputs = []
for i in range(n):
    inputs += [input("").split(" ")]
    
tree = []

for parent, node, direction in inputs:
    parent = int(parent)
    node = int(node)
    
    # initialize tree
    if tree == []:
        tree += [[parent]]
        
        tree += [['x'] * 2]
    
    # check if parent is in tree
    parent_level = 0
    parent_index = 'x'
    for index, level in enumerate(tree):
        if parent in level:
            # get parent_level
            parent_level = index
            # get parent_index
            parent_index = level.index(parent)
            break
    
    # add node
    if direction == "L":
        node_index = parent_index * 2
    elif direction == "R":
        node_index = (parent_index * 2) + 1
    # print(parent_level, node_index, parent, node)
    tree[parent_level + 1][node_index] = node
    # check if grandchild level exist
    if not len(tree) > parent_level + 2:
        # initialize child
        tree += [['x', 'x']]
        continue
    
    
    # add grandchild node
    # get grandchild level
    gran_level = parent_level + 2
    
    tree[gran_level].insert(node_index * 2, 'x')
    tree[gran_level].insert((node_index * 2) + 1, 'x')
    
for index, level in enumerate(tree):
    tree[index] = list(filter(lambda item: item != 'x', level))

tree = list(filter(lambda level: level != [], tree))

print(tree)
```
## Longest Common Subsequence
**Description**: Given two strings, find the length of their longest common subsequence (LCS). A subsequence is a sequence that appears in the same relative order but not necessarily contiguous.
### Solution
#### my solution
**Time of Completion**: 40 min.
**Complete**: False
```
n = int(input(""))
test_cases = [''] * n
for i in range(n):
    test_cases[i] = input('').split(" ")

def subsequence(string1, string2):
    if string1 == '' or string2 == '':
        return ""

    shortest_len =     
    
    for first_index, first_letter in enumerate(string1):
        for second_index, second_letter in enumerate(string2):
            print(string1, string2)
            print(first_letter, second_letter)
            if first_letter == second_letter:
                return first_letter + subsequence(string1[(first_index + 1):], string2[(second_index + 1):])
    return ""

for test_case in test_cases:
    # print(subsequence(test_case[0], test_case[1]))
    print(len(subsequence(test_case[0], test_case[1])))
    print("")
```

# Intermediate Problems
## Matrix Path Sum
**Problem Statement**: You are given an N x M matrix of integers, where each cell represents a value. You need to find the minimum path sum from the top-left corner (0,0) to the bottom right corner (N-1, M-1). You may only move down or right at any step.
### Solution
```
n, m = list(map(lambda x: int(x), input("Enter n m:").split(" ")))

print(f"Enter the {n} x {m} matrix:")

grid = []

for i in range(n):
    row = list(map(lambda x: int(x), input("").split(" ")))
    grid += [row[:m]]


def grid_paths(n, m):
    # base output
    if n == 0 and m == 0:
        return grid[n][m]
    if n == 0:
        return grid[n][m] + grid_paths(n, m - 1)
    if m == 0:
        return grid[n][m] + grid_paths(n - 1, m)
    
    # pointer comparison 
    left = grid[n][m - 1]
    top = grid[n - 1][m]
    
    if left < top:
        return grid[n][m] + grid_paths(n, m - 1)
    if top < left:
        return grid[n][m] + grid_paths(n - 1, m)
    
    return grid[n][m] + grid_paths(n - 1, m)

print(grid_paths(n - 1, m - 1))
```
