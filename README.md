## <pre>             IT 314 - Software Engineering </pre> 
### Lab 5 : Static Analysis
### Student Name : Kalp Pandya
### Student ID: 202001466

####  selected tool and github repo

I will be using pylint tool for python.<br/>
- **Github repo : https://github.com/MakeContributions/DSA.git**
<br/><br/>
![1](https://user-images.githubusercontent.com/77293195/227482175-91b9c76f-bd86-4b96-aafa-a9f4a93fdb94.png)
<br/><br/>
- **Installing tools**
<br/><br/>
![2](https://user-images.githubusercontent.com/77293195/227483682-8b89eb97-775e-40c2-a355-420a4ebfdfbe.png)
<br/><br/>
As we can see pylint already exists.
<br/>

### Performing static Analysis and error understanding

1.https://github.com/MakeContributions/DSA/blob/main/algorithms/Python/dynamic_programming/knapsack.py
<br/>Tool output: 
![4](https://user-images.githubusercontent.com/77293195/227483899-178b2b93-651c-4ee2-9963-6351ee4c0c8d.png)
<br/><br/>

2.https://github.com/MakeContributions/DSA/blob/main/algorithms/Python/dynamic_programming/fibonacci_series.py
<br/>Tool output: 

![5](https://user-images.githubusercontent.com/77293195/227484189-4f8421ae-d75b-4975-8997-20f4b235807a.png)
<br/><br/>

3.https://github.com/MakeContributions/DSA/blob/main/algorithms/Python/sorting/quicksort.py
<br/>Tool output: 

![6](https://user-images.githubusercontent.com/77293195/227484404-c274bf33-3801-4244-9258-2135fe36f4e3.png)
<br/><br/>

4.https://github.com/MakeContributions/DSA/blob/main/algorithms/Python/sorting/merge_sort.py
<br/>Tool output: 

![7](https://user-images.githubusercontent.com/77293195/227484475-fa59243a-933a-4e7f-830b-11e9adae70e8.png)
<br/><br/>

5.https://github.com/MakeContributions/DSA/blob/main/algorithms/Python/trees/binary_tree.py
<br/>Tool output: 

![8](https://user-images.githubusercontent.com/77293195/227484571-8c13b046-e617-4f30-acea-25dd7c0591c4.png)
<br/><br/>

6.https://github.com/MakeContributions/DSA/blob/main/algorithms/Python/strings/rabin-karp-algorithm.py
<br/>Tool output: 

![9](https://user-images.githubusercontent.com/77293195/227484804-9f955a02-7822-4cae-8c94-ba9b6941d668.png)
<br/><br/>

#### Understanding of errors: 
1) C0103: Variable does not confirm to snake_case naming style<br/>
    This error tells that the declared vairable is not according to snake_case naming convention.
2) C0303: Trailing whitespace at the end of a line
     This is caused when there is emtpy space at the end of line and before a new line.This space is unneccessary.
3) C0321: More than one statment on a single line<br/>
    This tells that multiple statements are written in the same line. This is not a good practice as the code will be more readable when single statement is there in a line.
4) C0114/C0ll6: Missing module docstring/function docstring <br/>
    This tells that the docstring is not specified for the modules or functions. The docstring is like a comment or some text description that is ingored by compiler but helps other people to understand the 
  purpose of module/function docstring. It is a good practice to write docstrings.
5) W0622: redefined-builtin <br/>
    This error tells about variables which are used when a variable or function override a built-in.
6) W0621: Redifining name from outerscope <br/>
    This error tells that the local variable name is same as that of one of global variable. This makes the local scope to use local version of the variable while hiding the global version
  of the variable.
7) R1705: Unneccessary else after return statement<br/>
    This is caused when an else statement is written after a "return" statement which is not executed anyhow.
8) R1722: Consider using 'sys.exit' instead <br/>
    This error tells to use the sys.exit(), instead of using exit() or quit().
 9) W0611: Unused imports
    This is caused when there are any modules or packages that are imported but not used.
