# Programming MCQs with Answers

## Q1. Which of the following is used to find and fix bugs in the Java programs?
- a) JVM  
- b) **JDB** ✅  
- c) JDK  
- d) JRE  

**Explanation:** The Java Debugger (JDB or jdb) is a command-line java debugger that debugs the java class.

---

## Q2. What was the initial name of Java when it was first developed for embedded systems?
- a) Bluenltk  
- b) **Oak** ✅  
- c) Java  
- d) Javac  

**Explanation:** Java was first called Oak, but before Oak, in prototype form, Gosling referred to it as “Greentalk” with .gt extension.

---

## Q3. What will be the output of the following program?

```java
class Question {
    int a = 40;
    int b = 20;
}
public class Child1 extends Question {
    int a = 100;
    int b = 200;
    void add(int a, int b) {
        System.out.println(a + this.b - super.a);
    }
    public static void main(String[] args) {
        Child1 c = new Child1(); 
        c.add(10, 30); 
    }
}
```
**If executed, output will be:**  
- a) 260  
- b) 130  
- c) 0  
- d) **170** ✅  

**Explanation:** a = 10, this.b = 200, super.a = 40 → 10 + 200 – 40 = 170.

---

## Q4. Which exception is thrown when an array element is accessed beyond the array size?
- a) ArrayElementOutOfBounds  
- b) **ArrayIndexOutOfBoundsException** ✅  
- c) ArrayIndexOutOfBounds  
- d) None of these  

**Explanation:** ArrayIndexOutOfBoundsException is thrown when an array element is accessed beyond the array size.

---

## Q5. What will be the output of the following program?

```java
import java.io.*;
public class Question {
    public static void main(String[] args){
         try {
             PrintWriter writer = new PrintWriter(System.out);
             writer.write("10"+ 6);
             writer.close();
        }
        catch (Exception e) {
             System.out.println(e);
        }
    }
}
```
- a) Compile-time error  
- b) Run-time error  
- c) 16  
- d) **106** ✅  

**Explanation:** "10" + 6 performs string concatenation, giving "106".

---

## Q6. Which operator is used for dynamic memory allocation in C++?
- a) **new** ✅  
- b) malloc  
- c) alloc  
- d) alloc_mem  

**Explanation:** In C++, `new` is used for dynamic memory allocation. `malloc` is from C.

---

## Q7. Which statement is true about C++ references?
- a) **References cannot be null** ✅  
- b) References can be re-assigned  
- c) References occupy more memory than pointers  
- d) References are used for dynamic memory allocation  

**Explanation:** References must be initialized and cannot be null or reassigned.

---

## Q8. What is the output of the following code snippet?

```cpp
#include <iostream>
using namespace std;
class A { 
public: 
    virtual void show() { cout << "A"; } 
};
class B : public A { 
public: 
    void show() override { cout << "B"; } 
};
int main() {
    A* ptr = new B();
    ptr->show();
}
```
- a) A  
- b) **B** ✅  
- c) Compilation Error  
- d) Undefined Behavior  

**Explanation:** Virtual function ensures derived class method is called. Output: B.

---

## Q9. What will be the output of the following code?

```cpp
#include <iostream>
using namespace std;
class X {
public:
    X() { cout << "X"; }
    ~X() { cout << "Y"; }
};
int main() {
    X* obj = new X();
    delete obj;
}    
```
- a) X  
- b) Y  
- c) **XY** ✅  
- d) YX  

**Explanation:** Constructor prints X, destructor prints Y. Combined: XY.

---

## Q10. If an integer needs two bytes of storage, then the minimum value of an unsigned integer in C would be
- a) -(2^16 -1)  
- b) **0** ✅  
- c) -(2^15 -1)  
- d) -2^15  

**Explanation:** Unsigned int minimum is always 0.

---

## Q11. The loop which is executed at least once is
- a) while  
- b) **do-while** ✅  
- c) for  
- d) none  

**Explanation:** `do-while` executes once before checking the condition.

---

## Q12. What is the best case and worst case complexity of ordered linear search?
- a) O(nlogn), O(logn)  
- b) O(logn), O(nlogn)  
- c) O(n), O(1)  
- d) **O(1), O(n)** ✅  

**Explanation:** Best case: element found at first → O(1). Worst case: last or absent → O(n).

---

## Q13. Which of the following statements is true about the equality of two structure variables?
- a) **Two structure variables are equal if all their members are equal** ✅  
- b) Equal if they have the same address  
- c) Cannot be compared  
- d) None  

**Explanation:** Struct variables are equal if all member values match.

---

## Q14. How many times 'Hello' will be printed?

```c
#include <stdio.h>
int main() {
    int i = 0;
    int j = 0;

    for (i = 0; i < 4; i++) {
        for (j = 0; j < 5; j++) {
            if (i > 0)
                continue;
            printf("Hello \n");
        }
    }
    return 0;
}
```
- a) 4 times  
- b) 20 times  
- c) **5 times** ✅  
- d) no print  

**Explanation:** Only when i=0 → prints 5 times.

---

## Q15. What is the output of the following code?

```c
#include <stdio.h>
void swap(int a, int b){
   int temp =  a;
   a = b;
   b = temp;
}
int main(){
   int x = 1, y = 2;
   swap(x, y);
   printf("x = %d, y = %d \n", x, y);
   return 0;
}
```
- a) **x = 1, y = 2** ✅  
- b) x = 2, y = 1  
- c) Compilation error  
- d) Runtime error  

**Explanation:** Pass-by-value means original variables unchanged.
