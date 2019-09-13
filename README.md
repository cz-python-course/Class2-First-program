# Class2 - First-program

Okay, so this is the time to start programming, right? YES! You can clone this project in repl.it using the url in your address bar (its [this](https://github.com/cz-python-course/Class2-First-program), if you want to make sure)
After you open the project the project in repl, you will find the main.py file. We will work on that file.

You can run it to see if it's working. but after that, delete everything in that file. We are going to work on it in a moment.

## But I don't know how to write anything yet!

I know, and it's okay. in every programming language, there are a few things you have to know to start creating your own programs. I like to compare those small things to lego blocks. You will need to connect one block into another, to create something big:

### How do I show something on the screen?

To do this, we use a funtion called **print()**. This command prints a string in the console for you.
```python
print('this is a text string')
```
We will use thos a lot in our programs, since this is the way we have to communicate with the user (without graphical interfaces).

### How do I store some information?
We saw that in previous classes. We can assing the result to a variable. and we can print the result later!
```python
result = 2 + 2
print(result)
```

### How do I expect the user to type something in my program?

To read the user input, we are going to use the function *input()*. This function will wait for the user input. When the user press <kbd>enter</kbd>, everything that was typed will return to you. You can assign it to a variable if you want to store the value. Since most of the time you will have to ask something in order to get a response for the user, the input function also allows us to pass a string to be printed:
```python
name = input('what is your name?')
print(name)
```

## Exercise

Ok, we learned a way to ask something, store the user answer, and print the result on the screen. In the end of this class we will have a program that asks for the name of the person, and how many cups of coffee the person drank in the last 3 days, and it will show the average number of cups of coffee.

The first thing we will do is break this problem in small steps:

1. Ask the name, and store the answer
2. Ask the # of cups 1 day ago, and store the answer
3. Ask the # of cups 2 day ago, and store the answer
4. Ask the # of cups 3 day ago, and store the answer
5. Calculate the average # of cups, and store it
6. Print the average # of cups.

### Step 1

We saw that the function to ask something is *input('question')*, so we will do this, saving the result into a variable called name:
```python
name = input('What is your name')
```

### Step 2

After storing the name, we will ask the user how many cups of coffee he/she drank 1 day ago:

```python
name = input('What is your name')
dayOne = input('How many cups of coffee you drank 1 day ago?')
```

### Step 3

The same as Step 2, but storing in another variable, and asking for the second day

```python
name = input('What is your name')
dayOne = input('How many cups of coffee you drank 1 day ago?')
dayTwo = input('How many cups of coffee you drank 2 days ago?')
```

### Step 4

The same as Step 2 and 3, but storing in another variable, and asking for the second day

```python
name = input('What is your name')
dayOne = input('How many cups of coffee you drank 1 day ago?')
dayTwo = input('How many cups of coffee you drank 2 days ago?')
dayThree = input('How many cups of coffee you drank 3 days ago?')
```

### Step 5

Now we have to calculate the average value, and store it. we also have to convert the answer to a number (python understand the user response as a text always)


```python
name = input('What is your name')
dayOne = input('How many cups of coffee you drank 1 day ago?')
dayTwo = input('How many cups of coffee you drank 2 days ago?')
dayThree = input('How many cups of coffee you drank 3 days ago?')
average = (int(dayOne) + int(dayTwo) + int(dayThree)) / 3
```

### Step 6

In the last step, we are going to show the result to the user

```python
name = input('What is your name')
dayOne = input('How many cups of coffee you drank 1 day ago?')
dayTwo = input('How many cups of coffee you drank 2 days ago?')
dayThree = input('How many cups of coffee you drank 3 days ago?')
average = (int(dayOne) + int(dayTwo) + int(dayThree)) / 3
print(average)
```

Okay, the result is being printed... But it's not really easy to understand what's the value. Of course we can print another line before, to show as result, but what if we want to print the result in the same line? We can *concatenate* the values. we also have to convert the average into a string to perform a concatenation

```python
name = input('What is your name')
dayOne = input('How many cups of coffee you drank 1 day ago?')
dayTwo = input('How many cups of coffee you drank 2 days ago?')
dayThree = input('How many cups of coffee you drank 3 days ago?')
average = (int(dayOne) + int(dayTwo) + int(dayThree)) / 3
print('the average is:' + str(average))
```
