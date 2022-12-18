# Section3: Vectors, Rotators, and Trigonometry

내적이랑 외적은 안다루네.. 흠..

## Table of Contents

1. Coordinates
2. Vectors 
3. Vector Examples
4. Vector Operations
5. Vector Operations Examples
6. Vector Magnitude
7. Vector Magnitude Examples
8. Vector Normalization
9. Rotators
10. Section 3 Challenge

---

1. Coordinates

    * **Scalar** - a single numerical value
    * X coordinate - position along the x axis
    * XY coordinates - position in the xy plane
        * Represented by an ordered pair
    * XYZ coordinates - position in 3-dimensional space
        * Represented by an ordered triple
    * (0, 0, 0) is the world **origin**
        * (0, 0) is the origin in 2-dimentional space

2. Vectors

    An arrow with a starting point and an ending point is known as a **vector**.  
    A vector contains two pieces of information a **direction** and a **magnitude**.

    A 2D vector has X and Y components.

    A vector v starting at A(5, 5) and ending at B(20, 20) is

    $\vec{\mathbf{v}} = (20 - 5, 20 - 5) = (15, 15)$

    We can have other vectors in this XY plane with different starting locations and ending locations,
    and it doesn't matter where we start them or end them if they're x and y components are all equal.
    These are all the same vector.
    All that matters is their direction and their magnitude.

    
3. Vector Examples

    $\vec{\mathbf{v}} = (x1, y1)$  
    then, the opposite directional vector of v is  
    $\vec{\mathbf{-v}} = -(x1, y1) = (-x1, -y1)$


4. Vector Operations

    * **Scalar Multiplication**(Vector Multiplicaiton by a Scalar)
    * **Vector Addition**
        * (x1, y1) + (x2, y2) = (x1 + x2, y1 + y2) (Component-wise addition)
    * **Vector Subtraction**
        * (x1, y1) - (x2, y2) = (x1 - x2, y1 - y2) (Component-wise subtraction)

5. Vector Operations Examples

    * Keep in mind that all positions are relative to the origin.

6. **Vector Magnitude**

    * Right Triangle -> Pythagorean Theorem -> Positive Square Root

7. Vector Magnitude Examples

    * If you know the location of two objects, you can determine the distance between them.


8. **Vector Normalization**

    * **Unit Vector**: Vector witha magnitude of 1
        It is useful when you want to show the direction of moving little by little, not instant movement in the game.  
        Also called a **normalized** vector.

9. Rotators

    * Left Hand vs Right Hand Coordinate Systems

        ![3-D Coordinate Systems](https://learn.microsoft.com/en-us/previous-versions/windows/desktop/images/bb324490.leftrght(en-us,vs.85).gif)

        Each game engine or library uses a different coordinate system.

    * **Rotators**

        * **Pitch**: Rotation about the Y axis
        * **Yaw**: Rotation about the Z zxis
        * **Roll**: Rotation about the X axis

        * Rotator: (Pitch, Yaw, Roll) (0~360)

10. Section 3 Challenge

Examples of vector operations that can be used in games.

    The enemy AI constantly adjusts the direction vector by referring to the character's position vector and direction vector to track the character.
