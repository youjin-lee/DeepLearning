---
title: "ch2.Linear Algebra (modifying)"
date: 2020-02-05 17:25:28 -0400
categories: deeplearning IanGoodfellow
---

## Abstract

선형대수(Linear algebra)는 과학, 공학에서 널리 쓰이는 수학의 한가지이다.

그러나 선형대수는 이산형(Discrete)보다는 연속형(Continous) 수학이기에 많은 데이터 사이언티스트들은 이에 대한 경험이 부족하다.

### "Good Understanding of Linear Algebra is essential for understading and working with many machine learning algorithms, especially deep learning algorithms."

그러므로 뒤의 내용을 학습하기 위해 전제조건이 되어야할 선형대수의 주요 포인트에 먼저 설명하겠다.

선형대수에 대해 사전지식이 있을 경우 가볍게 넘겨도 되며, 딥러닝에 필요한 부분들만 다뤘기 때문에 추가로 공부하는 것도 추천한다.

추천서적 : Matrix Cookbook(Petersen and Pedersen,2006)
  
----------------

## 2.1 Scalars, Vectors, Matrices and Tensors

The study of linear algebra involves several types of mathematical objects:

- Scalars

   just a single number.

  ![2_1](https://user-images.githubusercontent.com/27392019/73827577-250f7480-4843-11ea-9469-4c2db13d66bc.png)
  ![2_2](https://user-images.githubusercontent.com/27392019/73827581-280a6500-4843-11ea-9ad0-57296a96db44.png)

- Vectors

  an array of numbers(arranged in order). identify each individual number by its index in that ordering.
  
  ![2_3](https://user-images.githubusercontent.com/27392019/73829469-5473b080-4846-11ea-8a91-72eac2f89552.png)
  
  We can think of vectors as identifying points in space, with each element giving the coordinate along a different axis.
  
  ![2_5](https://user-images.githubusercontent.com/27392019/73830627-4faffc00-4848-11ea-9434-937b9eae4807.png)
  
  - 원소 접근 방법
  
    ![2_4](https://user-images.githubusercontent.com/27392019/73829548-7ff69b00-4846-11ea-8bc8-9b196e3f668e.png)
  

- Matrices

  a 2-D array of numbers.
  
  We can identify all the numbers with vertical coordinate i by writing a “:” for the horizontal coordinate.
  
  ![2_6](https://user-images.githubusercontent.com/27392019/73901863-576ab180-48d7-11ea-9b65-6c8243a30043.png)
  
  ![2_7](https://user-images.githubusercontent.com/27392019/73901864-589bde80-48d7-11ea-8aaa-28012957f540.png)
  

- Tensor

  an array with more than two axes.
  
  We identify the element of A at coordinates (i, j, k) by writing Ai,j,k
  
-----------------------------

- Transpose

  matrix across a diagonal line(called themaindiagonal).
  
  ![2_8](https://user-images.githubusercontent.com/27392019/73901868-59cd0b80-48d7-11ea-9339-52161abd969a.png)
  
  - Vectors
  
    Vectors can be thought of as matrices that contain only one column.
    Transpose of a vector is therefore a matrix with only one row.
    using the transpose operator to turn it into a standard column vector.
    
    ![2_9](https://user-images.githubusercontent.com/27392019/73901872-605b8300-48d7-11ea-8ba6-8a6fa49369a2.png)
  
  - Scalar
  
    A scalar can be thought of as a matrix with only a single entry. A scalar is its own transpose.
    
    ![2_10](https://user-images.githubusercontent.com/27392019/73901874-62254680-48d7-11ea-8414-944ed182c493.png)
    
    
-----------------------------------------------

- 행렬 덧셈

  add matrices to each other, as long as the same shape
  
  ![2_11](https://user-images.githubusercontent.com/27392019/73901877-63567380-48d7-11ea-9e46-edde750724c7.png)
  
  
- Scalar배, 덧셈

  add a scalar to a matrix or multiply a matrix by a scalar
  
  ![2_12](https://user-images.githubusercontent.com/27392019/73901879-65b8cd80-48d7-11ea-8f1e-2652b20c92c9.png)
  
### Broadcasting

In the context of deep learning, we also use some less conventional notation. the vector b is added to each row of the matrix. a matrix with b copied into each row before doing the addition.

![2_13](https://user-images.githubusercontent.com/27392019/73901882-681b2780-48d7-11ea-8517-7c1282f01af3.png)
