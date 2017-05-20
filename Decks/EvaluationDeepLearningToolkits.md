# Evaluation of Deep Learning Toolkits

There are a lot of deep learning libraries, each comes with its own flavour. This article compares the well-known Deep Learning toolkits along with the fundamental programming models.

##  Symbolic vs Imperative Programs

###  Symbolic Programs

Symbolic frameworks (such as CNTK, MXNET, TensorFlow, Theano) allow functions to be defined abstractly through computation graphs. In the symbolic style, we first express complex functions in terms of placeholder values. Then, we can execute these functions by binding them to real values. A large portion of deep learning libraries chose to be symbolic instead due to its efficiency, both in terms of memory and runtime. Symbolic computation is useful for several reasons:

1. Because we define a full computation graph before executing it, sophisticated optimizations can be performed to eliminate unnecessary or repeated work. This tends to give better performance than imperative programming. 
2. As therelationships between different variables are stored in the computation graph, we can then perform efficient auto-differentiation.


###  Imperative Programs

If you are a python/c++ programmer, you are already familiar with imperative programs. Imperative style programs (Torch, Caffe, etc.) conduct the computation as we run them. Imperative programs are usually more flexible than symbolic programs. Because imperative programs are actually more native than the symbolic ones, it is easier to use native language features and inject them into computation flow. 

The below tables describe and compare the commonly used open-source deep learning frameworks:

| Software | Creator | Platform | Software license | Open source | Interface | CUDA support | 
|:----------|:-------|:---------|:-----------------|:------------|:----------|:------------|
| CNTK | Microsoft Research | Linux, Windows | MIT | Yes | Python, C++, C# and CLI | Yes |
| TensorFlow | Google Brain Team | Linux, Mac OS X| Apache 2.0 | Yes | Python (Numpy), C/C++ | Yes |
| Theano | Universite de Montreal | Cross-platform | BSD license | Yes | Python | Yes | Yes |Yes |
| MXNET | Distributed (Deep) Machine Learning Community | Ubuntu, OS X, Windows, AWS, Android, iOS, JavaScript | Apache 2.0 | Yes | C++, Python, Julia, Matlab, JavaScript, R, Scala | Yes |
| Caffe | Berkeley AI Research | Linux, Mac OS X, Windows | BSD license | Yes | Python, Matlab | Yes |


| Software | Recurrent Nets | Convolutional Nets | RBMs |
|:---------|:---------------|:-------------------|:-----|
| CNTK | Yes | Yes | No |
| TensorFlow | Yes | Yes | Yes|
| Theano | Yes |Yes | Yes |
| MXNET | Yes | Yes | Yes |
| Caffe | Yes | Yes | Yes |
