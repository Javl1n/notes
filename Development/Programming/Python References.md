# General Functions
## map()
- w3school - https://www.w3schools.com/python/ref_func_map.asp
- codewars sample problem - https://www.codewars.com/kata/541c8630095125aba6000c00/solutions/python
```
def digital_root(n):
	return n if n < 10 else digital_root(sum(map(int,str(n))))
```

# String Functions
## format()
- w3school - https://www.w3schools.com/python/ref_string_format.asp
- codewars sample problem - https://www.codewars.com/kata/5266876b8f4bf2da9b000362/solutions/python
```
def likes(names):
	n = len(names)
	return {
		0: 'no one likes this',
		1: '{} likes this', 
		2: '{} and {} like this', 
		3: '{}, {} and {} like this', 
		4: '{}, {} and {others} others like this'
	}[min(4, n)].format(*names[:3], others=n-2)
```

## count()
- w3school - https://www.w3schools.com/python/ref_string_count.asp
- codewars sample problem - https://www.codewars.com/kata/54b42f9314d9229fd6000d9c/solutions/python
```
def duplicate_encode(word):
    return "".join(["(" if word.lower().count(c) == 1 else ")" for c in word.lower()])
```

# Number Functions
## sum()
- w3school - 
- codewars sample problem - https://www.codewars.com/kata/514b92a657cdc65150000006/train/python
```
def solution(number):
    return sum(x for x in range(number) if x % 3 == 0 or x % 5 == 0)  
```

# Loops
## Single line for loop
```
def array_diff(a, b):
    return [x for x in a if x not in b]
```