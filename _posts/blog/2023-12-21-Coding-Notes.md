---
layout: post
title: Coding Notes
categories: blog
description: Hey, this is my coding notes for python, langchain and gradio.
keywords: AI Papers, Publications
---
This blog records the problems I encountered and the knowledge I learned in software project development. The blog content includes programming knowledge such as Python coding standards, learning notes, and design philosophy.                                                                        

------------------------------------

## Python 
### Style Philosophy for Python Code
* One of coding's key sight is that code is read much**more often** than it is written. 

* "Readability counts！"

* Readability is much more important than code length & showing off coding skills & slight efficiency improvement.

* Consistency is the foundation of the readability.

   

#### Name Conventions




| Type                                  | Naming Conventions            | Example                       | PS                  |
| ------------------------------------- | ----------------------------- | ----------------------------- | ------------------- |
| **Class Names**                       | CapWords                      | Class Agent()：               | CapitalizedWords    |
| **Type Variable Names**               | CapWords                      | KT=TypeVar（'kT_contra',...） |                     |
| **Exception**                         | CapWords+“Error”              | KeyError                      | word +"Error"       |
| **Function Names** & **Method Names** | snake_case                    | def get_user_names():         | avoid abbreviations |
| **Variable Names**                    | snake_case                    | user_name、any_str、agent_num | short, simple，abbv |
| **Module(fIle.py)**                   | snake_case                    | agents.py、agent_define.py    | avoid abbreviations |
| **Package Names**                     | lowercase(prefer)、snake_case | pip install langchain         | folder names        |
|                                       |                               |                               |                     |
|                                       |                               |                               |                     |

**Special Name Conventions**

 [Link](https://peps.python.org/pep-0008/#descriptive-naming-styles)

|                                    | Conventions | Example                               | PS                     |
| ---------------------------------- | ----------- | ------------------------------------- | ---------------------- |
| **Constant**                       | UPPERCASE   | OPENAI_BASE                           | if long: _  OK         |
| **Class Private Variables\Method** | _snake_case | def _get_attr():                      | leading underscores    |
| **Instance Methods Arguments**     | self,...    | def get_abc(self,x):                  | first argument is self |
| **Class Method Arguments**         | cls,...     | @classmethod<br />def get_abc(cls,x): | first argument is cls  |
| **Conflict With Reserved Word**    | +"_"        | class\_, int\_                        |                        |
|                                    |             |                                       |                        |

#### Readability Promotion

* More is better.

  ```python
   #Correct:
  
  def foo(x):
      if x >= 0:
          return math.sqrt(x)
      else:
          return None
  
  def bar(x):
      if x < 0:
          return None
      return math.sqrt(x)
  # Wrong:
  
  def foo(x):
      if x >= 0:
          return math.sqrt(x)
  
  def bar(x):
      if x < 0:
          return
      return math.sqrt(x)
  ```

  

* Isinstance \> type.

  ```python
  # Correct:
  if isinstance(obj, int):
  # Wrong:
  if type(obj) is type(1):
  ```

* Don't compare values with True

  ```python
  # Correct:
  if greeting:
  # Wrong:
  if greeting == True:
  ```

* Use `''.startswith()` and `''.endswith()` instead of string slicing [-3:]==XXX in if conditions

  ```python
  # Correct:
  if foo.startswith('bar'):
  # Wrong:
  if foo[:3] == 'bar':
      
  ```



#### Optional Requirement

* Efficient concat of string
  
  ```python
  # Time complexity O(n)
  ''.join
  ```


### How Python Works

[Python Guide Doc ](https://developers.google.com/docs/api/quickstart/python)

### Grammar Knowledge Base



#### Union:

Union is a generics type in typing module in python，used to represent one of multiple types. In typing hinit, Union can be use to indicate that a variable can be one of multiple types. For example, Union [int, str] meaning that a variable may be int or string.

**Example **

```python
MessageLikeRepresentation = Union[
    MessageLike,
    Tuple[str, str],
    Tuple[Type, str],
    str,
]

# The code means that the type of MessageLikeRepresentation can be one of MessageLike, Tuple[str,str], tuple[Type, str] and str.
```
#### Tuple: Unchanged List

**Example for Union and Tuple**

```python
from typing import Union,Tuple,List

def testTuple(elem:Union[Tuple[str],List[str]]) -> Tuple:
    print(elem[0],elem[1])
    print(f"Index:{elem.index('elem0')}")
    # ValueError: 'elem0' is not in list
    print(f"Count:{elem.count('elem1')}")
print("Test tuple: ")
testTuple(("elem0","elem1"))
print("Test Union: ")
testTuple(["elem0","TestUnion1"])
print(Union[])
```
**Output**
```
Test tuple: 
elem0 elem1
Index:0
Count:1
Test Union: 
elem0 TestUnion1
Index:0
Count:0
```
**PS: Union in Typing is completely different from union method in set**
**Union() method：**

``` python
### union method in set
def test_union_method_in_set():
    x={"a","b","c"}
    y={"d","e","f"}
    z={"1","2","3"}
    print(z.union(x,y))
    # Output：{'b', 'a', '1', 'f', 'c', '3', '2', 'd', 'e'}
```



#### Try Catch

```python
# Correct:
try:
    value = collection[key]
except KeyError:
    return key_not_found(key)
else:
    return handle_value(value)
# Wrong:
try:
    # Too broad!
    return handle_value(collection[key])
except KeyError:
    # Will also catch KeyError raised by handle_value()
    return key_not_found(key)
```

#### Async : Asynchronous (Coroutine)

```python

import asyncio

async def task1():
    print("Task 1 started")
    await asyncio.sleep(2)
    print("Task 1 completed")

async def task2():
    print("Task 2 started")
    await asyncio.sleep(1)
    print("Task 2 completed")

async def main():
    await asyncio.gather(task1(), task2())

# 在异步环境中运行主函数
asyncio.run(main())

# Main started
# Task 1 started
# Task 2 started
# Task 3 started
# Task 3 completed
# Task 2 completed
# Task 1 completed         /3.1s 
```

<!-- ## References -->

<!-- [Reference] -->





#### How Import Works

##### How Python Works?

*  **Python  is a dynamic, interpreted（bytecode-compiled）language.**

##### As a result

* As a result, there is no type declarations of variables, parameters, functions, or methods in source code. Python tracks the types of all values at runtime **（Rather Than Compiled Time）** and flags code that does not make sense **at run**. 


```python
def main():
    if name == 'Guido':
        print(repeeeet(name) + '!!!')
        ### Only show errors at runtime
    else:
        print(repeat(name))

```



*  If you run a python script, Python interpreter will act as follow steps. For, example, if you run a piece of following code.



```cmd
project/
|-- run.py
|-- A/
|   |-- __init__.py
|   |-- a.py
|-- B/
|   |-- __init__.py
|   |-- b.py
### run 
~/(py38) python ~/project/run.py
```

* The order in which the interpreter searches for modules is described as **a sequence of steps.** 



1. **Current Working Directory (`'~'`):** The directory from which the script is executed is checked first. If the module is found there, it is imported.

2. **Script‘s Directory (`~/project/`):**The directory of the python script

3. **PYTHONPATH Environment Variable**: If the PYTHONPATH environment variable is set, the directories specified in it are searched next. Modules found in these directories are considered. **PS: In the Visual Studio Code (VSCode),when open the project in workspace,the"`${workspace}/src`" sub-floder will be automatically added as PYTHONPATH **

4. **Standard Library:** The interpreter then checks the standard library modules, which are part of the Python distribution.

5. **Built-in Modules（内置模块）:** Python has a set of built-in modules that are always available. These are searched next.

6. **Site Packages:** Finally, the interpreter looks in the directories specified by the site-packages directory, where third-party packages installed using tools like pip reside.

   



##### How `__init__.py` works?

1. **Initialization in `__init__.py`:**

   Suppose `__init__.py` in the `my_package` directory contains the following code:

   ```python
   pythonCopy code# my_package/__init__.py
   
   print("Initializing my_package")
   
   # Additional initialization code or configuration can go here
   ```

   When you import `my_package`, the code in `__init__.py` will be executed:

   ```python
   pythonCopy codeimport my_package
   # Output: Initializing my_package
   ```

2. Simple but easy to forget. [ref](https://blog.csdn.net/qq_37249443/article/details/108783599)

   ```python
   studio
       tools
           __init__.py
           camera
               __init__.py
               camera.py
           element
               __init__.py
               element.py
   ```

   ```python
   from studio import tools
       
   tools.camera.fn()
   tools.CameraNode('')
   tools.element.fn()
   ```

   

   If you have a studio/tools/`__init__.py` file like this:

   ```py
   from tools.camera import *
   from tools.element import *
   ```

   Then you can do a single import elsewhere like:

   ```py
   from studio import tools
   ## if you want to do tools.camera then you must import camera in the __init__.py
   ```

   and then reference everything as if it were directly in studio.tools. An `__init__.py` file allows you to treat any directory as a Python package. It is not necessary to write anything in the file itself, just creating it in your directory is enough. if you want to access Python files in sub-directories as well, then you must import those in the `__init__.py` of the parent directory.

3.  This is done to prevent directories with **a common name, such as string, utils, re**

4. In the simplest case, __init__.py can just be an empty file, but it can also **execute initialization code** for the package or set the __all__ **variable, described later.**

##### Import Python Scripts In Terminal - PYTHONPATH

* ```cmd
  export PYTHONPATH="XXXX" ## temporary and harmless
  ```

##### Import Python File in Vscode

![image-20231226002653851](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231226002653851.png)

![image-20231226002919575](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231226002919575.png)

**Project Organization**

![image-20231226003435377](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231226003435377.png)

**Code Snippet**

![image-20231226003614245](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231226003614245.png)

##### Vscode Setting In Python Project

![image-20231226004401254](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231226004401254.png)

###  How Error Traceback Work？

` Philosophy Of Debug`

##### Error Stack

How to find bugs in traceback elegently ？





###### Example

There is a error  traceback, which was found in openai module. The first question is - how to locate the bug？

This is project organization.

```properties
Agent_UI.py
- agents
  main_chat_agent.py (called)
  ....
....
```



Here is the error traceback.

> * File **"Agent_UI.test.py",** line 37, in <module>  for chunk in response:<font color=red> PS：The top stack: a possible error location</font>
>
> * File **"Agent_UI.test.py",** line 32, in outer_yield
>    for chunk in inner_stream:
>
> * File **"/home/ckq/ckq_2023/2023_12/AgentThinkTank/src/agents/main_chat_agent.py",** line 32, in stream
>    for chunk in self.chat_model.stream(self.messageHistory): 
>
> * File **"/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/langchain_core/language_models/chat_models.py",** line 244, in stream raise e
>
> * File **"/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/langchain_core/language_models/chat_models.py"**, line 228, in stream**for chunk in self._stream(
>   **
>
> * **File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/langchain_community/chat_models/openai.py", line 394, in _stream** for chunk in self.completion_with_retry(
>
> * <font color=red>The Agent_UI called the stream function in main_chat_agent.py. **But the last called function didn't mean that the error was located at here.**</font>
>
> * File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/langchain_community/chat_models/openai.py", line 360, in completion_with_retry
>   ​    return_completion_with_retry(\*\*kwargs)
>
> * File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/tenacity/__init__.py", line 289, in wrapped_f
>   ​    return self(f, *args, kw)
>
> * *File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/tenacity/__init__.py", line 379, in __call__
>   ​    do = self.iter(retry_state=retry_state)
>
> * *File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/tenacity/__init__.py", line 314, in iter
>   ​    return fut.result()
>
> * *File "/home/ckq/miniconda3/envs/py38/lib/python3.8/concurrent/futures/_base.py", line 437, in result
>   ​    return self.__get_result()
>   _
>
> * *_File "/home/ckq/miniconda3/envs/py38/lib/python3.8/concurrent/futures/_base.py", line 389, in __get_result
>   ​    raise self._exception
>   __
>
> * *__File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/tenacity/__init__.py", line 382, in __call__
>   ​    result = fn(*args, \*\*kwargs)
>
> * File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/langchain_community/chat_models/openai.py", line 358, in _completion_with_retry
>   ​    return self.client.create(\*\*kwargs)
>   _
>
> * _File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/openai/api_resources/chat_completion.py", line 25, in create
>   ​    return super().create(*args, \*\*kwargs)
>
> * _File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/openai/api_resources/abstract/engine_api_resource.py", line 153, in create
>   ​    response, _, api_key = requestor.request(
>
> * _File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/openai/api_requestor.py", line 298, in request
>   ​    resp, got_stream = self._interpret_response(result, stream)
>
> * File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages**/openai/**api_requestor.py", line 700, in _interpret_response
>   ​    self._interpret_response_line(
>
> * File "/home/ckq/miniconda3/envs/py38/lib/python3.8/site-packages/openai/api_requestor.py", line 763, in _interpret_response_line
>   ​    raise self.handle_error_response(
>   openai.error.InvalidRequestError: Unrecognized request argument supplied: modelType 
>
>   <font color=red>The most important information. Python found wrong type of argument. But it didn't mean that the error located at the superlink the traceback gived. </font>



<font color=red>In last information, we found that two keyword: **“modelType”** and **Unrecognized Request Arguments**. So the most efficient method to find error is: </font>

* Search **"modelType"**  key in **agent_UI.py** and **main_chat_agent.py**. (modelType)
* Look up the Function Calls / Class Instantiation in both file. (Unrecognized Request Arguments)



<font color=red> Assisting Methods include </font>

* Look up the `__init__` arguments (class/function).
* Look up the openai's class.



So, how the traceback was generated?

##### How is the traceback generated？

The traceback is generated with following steps：



>1. **Exception Triggering:** An exception occurs during program execution, which could be due to faulty code, invalid input, or other issues.
>2. **Exception Propagation:** The exception propagates from its occurrence point until it encounters a handler (e.g., a try-except block) or until the program terminates.
>3. **Traceback Generation:** When an exception goes unhandled and reaches the top level, Python generates a `traceback` object containing detailed information about the exception, such as the type, error message, and the call stack.
>4. **Traceback Analysis:** Developers can examine the `traceback` to understand where the exception occurred and how it propagated. The call stack information shows where the exception originated and the context of each call.

In traceback, following information is provided. And  the philosophy of debug is ：

| **Type**                    | **Example**                       | Explanation                                                                                                                                         | Methods of Debug                                                                                                                                                         |
| --------------------------- | --------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Exception Type:**         | **Unrecognized request argument** | Check the beginning of the traceback, which typically includes the exception type and error message. This helps identify the nature of the problem. | Most important information.                                                                                                                                              |
| **Call Stack Information:** | **Stack1 -Stack2 - ....**         | Extract the function call **sequence and positions from the traceback.** Traversing the traceback helps pinpoint the location of the error.         | Search from your own files \ Sometimes error isn't from the bottom stacks. The error may be transferred to bottom an than found in bottom.（python have not type check） |
| **File and Line Numbers:**  | **Agent_UI.py  & lineXXX**        | The traceback provides the file name and line number where the error occurred, facilitating quick identification of the problematic code.           | Please do not blindly  believe line number and offered links. Because the line numbers indicate the path of calling functions rather than the error locations            |
| **Context Information:**    | **modelType**                     | Tracebacks may also include additional context, such as the values of local variables, aiding further in the debugging process.                     | Search key words                                                                                                                                                         |
## pip conda

### pip

```cmd
## install this package
pip install -e .
```




## References


[1] ([SEP8 \ PEP 8 – Style Guide for Python Code | peps.python.org --- PEP 8 – Python 代码风格指南 | peps.python.org]

[2] Barry’s GNU Mailman style guide http://barry.warsaw.us/software/STYLEGUIDE.txt

[3] Donald Knuth’s The TeXBook, pages 195 and 196.

[4] http://www.wikipedia.com/wiki/CamelCase

[5] Typeshed repo https://github.com/python/typeshed


## Copyright
This document has been placed in the public domain.

[SEP8_Link](https://peps.python.org/pep-0008/#naming-conventions))
