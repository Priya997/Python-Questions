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
