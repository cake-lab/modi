---
title: Cloud-based or On-device&#58; An Empirical Study of Mobile Deep Inference
authors: Tian Guo
authors_list: 
  - tian
pdf_location: http://tianguo.info/publications/18ic2e_mobiledl.pdf
journal: 2018 IEEE International Conference on Cloud Engineering (IC2E'18) 
excerpt_separator: <!--more-->
publication_date: 04-17-2018

layout: post

---

Modern mobile applications benefit significantly from the advancement in deep learning, e.g., implementing real-time image recognition and conversational system. Given a trained deep learning model, applications usually need to perform a series of matrix operations based on the input data, in order to infer possible output values. Because of computation complexity and size constrained, these trained models are often hosted in the cloud. When utilizing these cloud-based models, mobile apps will have to send input dat over the network. While cloud-based deep learning can provide reasonable response time for mobile apps, it also restricts the use case scenarios, e.g. mobile apps need to have access to network. With mobile specific deep learning optimizations, it is now possible to employ on-device inference. However, because mobile hardware, e.g. GPU and memory size, can be very limited when compared to desktop counterpart, it is important to understand the feasibility of this new on-device deep learning inference architecture. In this paper, we empirically evaluate the inference efficiency of three Convolutional Neural Networks using a benchmark Android application we developed. Our measurement and analysis suggest that on-device inference can cost up to two orders of magnitude response time and energy when compared to cloud-based inference, and loading model and computing probability are two performance bottlenecks for on- device deep inferences.