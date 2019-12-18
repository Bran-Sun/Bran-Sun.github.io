---
layout: page
title: Project
---

Last update: Dec. 2019

## Current Projects
---

#### Blockgraph: A Scalable Alternative To Blockchain

* Introduction: Bitcoin is a digital currency system where different parties can make, re- ceive and verify payment. However, Bitcoin is limited to low throughput because of the propagation delay and limited block size.

* Motivation: Locality Principle. A locality can be any group of people who will transact within the group to a greater extent than outside the group. For example, people in the same place, company, organization.

* Method: The Blockgraph splits the blockchain into a global chain and multiple local chains. Every locality has its own chain and all local chains are synchronized to the global chain. If an end user wants to spend money in another locality, she has to transfer her money to that locality first.

* My contributions:
	1. implemented Blockgraph based on Bitcoin-0.11
	2. designed part of protocols and consensus mechanism
	3. conducted mathematical analysis about the security of Blockgraph

You can read the <a href="../public/doc/blockgraph.pdf">poster</a> to better understand our project.

#### Implement GPU driver(Raspi3) for rCore

* Introduction: <a href="https://github.com/rcore-os/rCore">rCore</a> is an OS kernel developed in Rust in Tsinghua University. Our project aimed at transplanting the drivers for Videocore IV on Raspi3 to rCore as well as the OpenGL library.

* Method: Like Mesa, our driver is splited into two parts. To hide the address of GPU memory from user, we replace them with offset in user space. When switching to kernel space, we calculate the actual address using offset and put them back into BCL/RCL.

* Result: Users are able to write C program to draw objects with the OpenGL ES library. And the following picture is when we ran our codes on Raspi3.

<img src="../public/img/rcore_driver.PNG" width="800" />


## Past Projects
---
#### GPU Sparse

* Introduction: TACO(The Tensor Algebra Compiler) is a fast and versatile library for tensor algebra. We want to parallelize the computation of sparse tensor computation by unfolding every dimension of the tensor and segmentedly sorting them using GPU.

* Result: our system performs seven times better than TACO(We optimized TACO by enabling it for multi-thread computation for sparse tensor) on computation speed.

