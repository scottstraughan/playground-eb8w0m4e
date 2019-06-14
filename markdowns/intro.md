# Introduction to SYCL

## What is SYCL?

SYCL enables developers to integrate parallel computing into your application and accelerate your code across OpenCL devices such as GPUs. Applications that require a large number of common operations can make huge performance improvements by running the operations in parallel on OpenCL devices. For example, the neural networks used in machine learning perform huge numbers of matrix operations and SYCL can be used to run these operations in parallel, vastly increasing performance and reducing the power consumption of the application.

With SYCL you can write code once and execute on a range of OpenCL enabled devices reducing your development effort. Develop with standard C++ and re-use your existing C++ libraries. There are also a number of frameworks including SYCL-DNN, ParallelSTL and SYCL-BLAS that harness SYCL to provide accelerated libraries and frameworks.

SYCL is a royalty-free open standard produced by the Khronos Group, the standards body responsible for other well known standards such as OpenGL, Vulkan or OpenCL. SYCL defines a high-level single source C++ programming for programming heterogeneous architectures such as GPUs, FPGAs, DSPs and other kinds of accelerators.

SYCL is single source, which means that rather than having your host side code and the kernel code (code which is compiled for an OpenCL device) defined separately as is the case with OpenCL, you have both your host code and kernel code in the same C++ source file. This opens up users to a range of benefts such as stronger type safety and templated kernel code.

## This Tutorial

This tutorial aims to teach you how to write a basic application that uses SYCL. It will cover how to discover a device to execute work on, different ways to express parallelism, how to manage your data and much more.
