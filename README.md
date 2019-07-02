# List of Python-Questions
I will be posting multiple choice Python questions here, which will be updated by me weekly!

From basic to advanced: test how well you know Python, refresh your knowledge a bit, or prepare for your coding interview! 💪 🚀 

Last update: 3 July'19

The answers are in the collapsed sections below the questions, simply click on them to expand it. Good luck ❤️


---

###### 1. What's the output?

```python
def hello(k):
    k = [1]

x = [0]
hello(x)
print(x)

```

- A: [0]
- B: [1]
- C: [1,0]
- D: [0,1]

<details><summary><b>Answer</b></summary>
<p>

#### Answer: A

A new list object is created within the function and after coming out of the function the reference is lost. This is an example of call by value where the value is updated withing the function. 
</p>
</details>

---

###### 2. What's the output?

```python
str1= '{3},{1} and {0}'. format('p','r','i')
print(str1)
```

- A: Tuple index out of range 
- B: i,r and p
- C: ppp,r
- D: None

<details><summary><b>Answer</b></summary>
<p>

#### Answer: A

We have only three characters in the tuple and as we know the indexing will start from 0. By which 'p' has 0 index, 'r' has 1 index and 'i' as two index.  String function format takes a format string and an arbitrary set of positional and keyword arguments. So, when we give give {3} it shows index out of range. For better understanding check next question.
</p>
</details>

---

###### 3. What's the output?

```python
str1= '{1},{1},{2} and {0}'. format('p','r','i')
str2 = '{0}{1}{0}'.format('priya', 'cad')
print(str1,str2)

```

- A: r,r,i,p priyacad0 
- B: r,r,i and p priyacad0
- C: r,r,i and p priyacadpriya
- D: p,p,r and i priyacadpriya

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

String function format takes a format string and an arbitrary set of positional and keyword arguments. For str1 ‘p’ has index 0, ‘r’ has index 1 and ‘i’ has index 2 and index 1 is used twice at firt and the second position. Whereas, str2 has only two indices 0 and 1. Index 0 is used twice at 1st and 3rd position.
</p>
</details>

---

###### 4. What's the output?

```python
a=3
b=3.876
c= -5
str1 = '{0:.4f} {0:3d} {2} {1}'.format(a, b, c)
print(str1)

```
Here, hash(#) represent spaces.

- A: 3.0000 3 -5 3.876
- B: 3 3.876 -5 3.876
- C: 3.0000 ###3 -5 3.876
- D: 3.0000 ##3 -5 3.876

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

At Index 0, integer a is formatted into a float with 4 decimal points, thus 3.0000. At Index 0, a = 3 is formatted into a integer with three blank spaces in front, thus it remains to '###3'. Index 2 and 1 values are picked next, which are -5 and 3.876 respectively. Here, '3' in '3d' is used as a right adjust flag. If we replace '3d' with '{0:-3d}' then it will become '3###' like this. 
</p>
</details>

---
###### 5. What's the output?

```python
line1='And here you can learn '
line2='You will fall in love with python '
line3='Pyhton is interpreted language '
line4=line1 + line2 + line3
print(line1.find('you'),line4.count('python'))

```
- A: 9,2
- B: 9 1
- C: (9,1)
- D: True,1

<details><summary><b>Answer</b></summary>
<p>

#### Answer: B

‘you’ is at Index 9 in Line1, find() returns the index of substring if found in the string Line1. count() returns the total number of occurences of the substring. Line4 is concatenated string from Line1, Line2 and Line3. We got only one occurrence because python is case sensitive language and one 'python' has 'P' in uppercase, we are looking for the exact match.

</p>
</details>

---
