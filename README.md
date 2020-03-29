Python 3.8.2 (tags/v3.8.2:7b3ab59, Feb 25 2020, 22:45:29) [MSC v.1916 32 bit (Intel)] on win32
Type "help", "copyright", "credits" or "license()" for more information.
>>> def create_cubes(n):
	result = []
	for x in range(n):
		result.append(x**3)
	return result

>>> create_cubes(10)
[0, 1, 8, 27, 64, 125, 216, 343, 512, 729]
>>> for x in create_cubes(10):
	print(x)

	
0
1
8
27
64
125
216
343
512
729
>>> def create_cubes(n):
	for x in range (n):
		yield x**3

		
>>> list(create_cubes(10))
[0, 1, 8, 27, 64, 125, 216, 343, 512, 729]
>>> def gen_fibon(n):

	a = 1
	b = 1
	for i in range(n):
		yield a
		a,b = b,a+b

		
>>> for number in gen_fibon(10):
	print(number)

	
1
1
2
3
5
8
13
21
34
55
>>> 
