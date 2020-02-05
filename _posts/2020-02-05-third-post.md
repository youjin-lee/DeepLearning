---
title: "ch2.Linear Algebra"
date: 2020-02-05 17:25:28 -0400
categories: deeplearning IanGoodfellow
---

<Abstract>
  
  선형대수(Linear algebra)는 과학, 공학에서 널리 쓰이는 수학의 한가지이다.\n
  
  그러나 선형대수는 이산형(Discrete)보다는 연속형(Continous) 수학이기에 많은 데이터 사이언티스트들은 이에 대한 경험이 부족하다.
  
  ### "Good Understanding of Linear Algebra is essential for understading and working with many machine learning algorithms, especially deep learning algorithms."
  
  그러므로 뒤의 내용을 학습하기 위해 전제조건이 되어야할 선형대수의 주요 포인트에 먼저 설명하겠다.
  
  선형대수에 대해 사전지식이 있을 경우 가볍게 넘겨도 되며, 딥러닝에 필요한 부분들만 다뤘기 때문에 추가로 공부하는 것도 추천한다.
  
  추천서적 : Matrix Cookbook(Petersen and Pedersen,2006)
  
----------------

## 2.1 Scalars, Vectors, Matrices and Tensors

The study of linear algebra involves several types of mathematical objects:

- Scalars

- Vectors

- Matrices

- Tensor


You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

​```python
def print_hi(name):
  print("hello", name)
print_hi('Tom')
​```

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
