# Section4: C++ in Unreal Engine


## Table of Contents

1. [Integrated Development Environment(IDE)](#integrated-development-environmentide)
2. [Setting up Visual Studio](#setting-up-visual-studio)
3. [C++ Refresher](#c-refresher)
4. [Reflection and Garbage Collection](#reflection-and-garbage-collection)
5. [Section 4 Challenge](#section-4-challenge)

---

### Integrated Development Environment(IDE)

I am using Visual Studio in Windows environment. :D

### Setting up Visual Studio

[Unreal Engine - Setting up Visual Studio](https://docs.unrealengine.com/5.1/en-US/setting-up-visual-studio-development-environment-for-cplusplus-projects-in-unreal-engine/)

* Start Visual Studio -> 'Continue without code'

* Tools -> Options
    * -> Environmet -> General -> Color Theme
    * -> Projects and Solutions -> General -> Uncheck 'Always show Error List if build finishes with errors'
    * -> Text Editor
        * -> All languages -> Scroll Bars -> 'Behavior' -> Check 'Use map mode for vertical scroll bar'
        * -> C/C++ 
            * -> Advanced
                * -> 'Browsing/Navigation' -> 'Hide External Dependencies Folders' ==> True
                * -> 'IntelliSense' -> 'Disable IntelliSense' ==> False
            * -> View
                * -> 'Inactive Code' -> 'Show Inactive Blocks' ==> False
    * -> Debugging -> General -> Uncheck 'Enable Edit and Continue and Hot Reload'

* Menubar -> Right Click
    * -> Customize -> Commands -> Toolbar -> Standard -> Preview -> 'Solution Configurations' -> Modify Selection -> 'Width' ==> 200

#### Testing Codes

* File -> New -> New Project -> 'Empty Project' -> Add -> Soure.cpp

    ```c++
    #include <iostream>

    int main()
    {
        std::cout << "Testing VS 2022!";
    }
    ```

* In Debug Mode -> Click 'Local Windows Debugger'


### C++ Refresher

#### **Classes** and **Inheritance**

* UObject
    * store data
    * cannot be placed in a level
* AActor
    * can be placed in the level
    * can have a visual representation
* APawn
    * can be possessed by a controller
* ACharactor
    * has a character movement component
    * has Character-specific functionality

#### 'Is A' vs 'Has A' Relationships

**Is A**
* Parent Class
    * a Parent **is not a** Child
    * a Parent **is not a** Grandchild
* Child Class
    * a Child **is a** Parent
    * a Child **is not a** Grandchild
* Grandchild Class
    * a Grandchild **is a** Child
    * a Grandchild **is a** Parent

---

**Has A**
* Outer Class
    * Inner Class
        * Inner Inner Class

    ---

* Package

    These Are Not SubObjects.
    * Meshes
    * Textures
    * Sound Files
    * ...

    These Are SubObjects. (Member Variable)
    * World
        * Level
            * Actor
                * Component

### Reflection and Garbage Collection

Tools Used By Unreal Engine

[Sparse Class Data](https://docs.unrealengine.com/5.1/en-US/sparse-class-data-in-unreal-engine/)

#### **Reflection**

Reflection is the ability of a program to examine itself at runtime.

#### **Garbage Collection**

사실 이해 잘 안됐는데 일단 넘어감..

### Section 4 Challenge

이건 C++ 복습하면서 정리해보는 걸로.