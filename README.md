# 📌 Project 8: String Library (OOP)

## 🔹 Overview
This project was implemented as part of **Course 10** in the **Programming Advices Track (https://programmingadvices.com/)** by **Dr. Mohammed Abu-Hadhoud**.  

The main idea is to **reuse all the string-related functions** we built earlier in **Course 7 – Algorithms & Problem Solving Level 3**, but instead of rewriting them, we collected them inside a **separate header file** (`clsString.h`) and wrapped them in a **class** to apply **Object-Oriented Programming (OOP) principles**.

---

## ✨ Features
- ✅ **Reusability**: No need to rewrite string functions; they are all encapsulated in one class.  
- ✅ **Encapsulation**: The internal implementation of each function is hidden, so we can call methods directly on the object without worrying about their internal logic.  
- ✅ **Static Functions**: Functions can be used directly without creating an object.  
- ✅ **Overloading**: We created overloaded functions – one that takes parameters and another that works directly on the object’s value. This makes updates easy: if we modify a function, all dependent functions benefit automatically.  
- ✅ **Flexibility**: Developers can either use class objects or call the static functions directly.  

---

## 📂 Project Structure
📁 Project-8-String-Library-OOP

 clsString.h # Header file containing the clsString class and all functions

 main.cpp # Sample code to demonstrate usage

 README.md # Project documentation


---

## 🧾 Sample Demonstration
Here are some examples from the `main.cpp` file:

```cpp
#include <iostream>
#include "clsString.h"
using namespace std;

int main()
{
    clsString String1("Sami yahya");

    cout << "String1 = " << String1.Value << endl;
    cout << "Number of words: " << String1.CountWords() << endl;

    String1.UpperFirstLetterOfEachWord();
    cout << "After Capitalizing First Letters: " << String1.Value << endl;

    String1.ReverseWordsInString();
    cout << "Reversed Words: " << String1.Value << endl;

    cout << "After Replace: " << String1.ReplaceWord("Sami", "Hamza") << endl;

    return 0;
}
```

---

## 🖥️ Example Output:
String1 = Sami yahya

Number of words: 2

After Capitalizing First Letters: Sami Yahya

Reversed Words: Yahya Sami

After Replace: Yahya Hamza


---


##  Acknowledgments

This project is part of the Programming Advices Training Track led by
- 👨‍🏫 Dr. Mohammed Abu-Hadhoud
- 📚 Platform:  [ProgrammingAdvices](https://programmingadvices.com/).
