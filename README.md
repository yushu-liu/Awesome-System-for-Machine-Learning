# Awesome-System-for-Machine-Learning[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of research in machine learning system. Link to the code if available is also present. I also summarize some papers if I think they are really interesting.

I categorize them by myself. You are kindly invited to pull requests!

## Table of Contents
### Resources
- [Book](#book)
- [Video](#video)
- [Course](#course)
- [Survey](#survey)
- [Tools](#userful-tools)
- [Project with code](#project)
### Papers
- [Model Deployment](#model-deployment-papers)
- [Inference Optimization](#machine-learning-system-papers-inference)
- [Distributed Training](#machine-learning-system-papers-training)
- [Resource Management](#resource-management)
- [Deep Reinforcement Learning system](#deep-reinforcement-learning-system)
- [Edge AI](#edge-or-mobile-papers)
- [Video System](#video-system-papers)
- [Advanced Theory](#advanced-theory)
- [Traditional System Optimization](#traditional-system-optimization-papers)

## Book

- Computer Architecture: A Quantitative Approach [[Must read]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.115.1881&rep=rep1&type=pdf)
- Streaming Systems [[Book]](https://www.oreilly.com/library/view/streaming-systems/9781491983867/)
- Kubernetes in Action (start to read) [[Book]](https://www.oreilly.com/library/view/kubernetes-in-action/9781617293726/)

## Video

- A New Golden Age for Computer Architecture History, Challenges, and Opportunities. David Patterson [[YouTube]](https://www.youtube.com/watch?v=uyc_pDBJotI&t=767s)
- How to Have a Bad Career. David Patterson (I am a big fan) [[YouTube]](https://www.youtube.com/watch?v=Rn1w4MRHIhc)
- SysML 18: Perspectives and Challenges. Michael Jordan [[YouTube]](https://www.youtube.com/watch?v=4inIBmY8dQI&t=26s)
- SysML 18: Systems and Machine Learning Symbiosis. Jeff Dean [[YouTube]](https://www.youtube.com/watch?v=Nj6uxDki6-0)

## Course

- CS294: AI For Systems and Systems For AI. [[UC Berkeley]](https://github.com/ucbrise/cs294-ai-sys-sp19) (*Strong Recommendation*)
- CSE 599W: System for ML.  [[Chen Tianqi]](https://github.com/tqchen) [[University of Washington]](http://dlsys.cs.washington.edu/)
- CSE 291F: Advanced Data Analytics and ML Systems. [[UCSD]](http://cseweb.ucsd.edu/classes/wi19/cse291-f/)
- CSci 8980: Machine Learning in Computer Systems [[University of Minnesota, Twin Cities]](http://www-users.cselabs.umn.edu/classes/Spring-2019/csci8980/)

## Survey

- Hidden technical debt in machine learning systems [[Paper]](https://papers.nips.cc/paper/5656-hidden-technical-debt-in-machine-learning-systems.pdf)
  - Sculley, David, et al. (*NIPS 2015*)
  - Summary: 
- End-to-end arguments in system design [[Paper]](http://web.mit.edu/Saltzer/www/publications/endtoend/endtoend.pdf)
  - Saltzer, Jerome H., David P. Reed, and David D. Clark. 
- System Design for Large Scale Machine Learning [[Thesis]](http://shivaram.org/publications/shivaram-dissertation.pdf)
- Deep Learning Inference in Facebook Data Centers: Characterization, Performance Optimizations and Hardware Implications [[Paper]](https://arxiv.org/pdf/1811.09886.pdf)
  - Park, Jongsoo, Maxim Naumov, Protonu Basu et al. *arXiv 2018*
  - Summary: This paper presents a characterizations of DL models and then shows the new design principle of DL hardware.

## Userful Tools

- Intel® VTune™ Amplifier [[Website]](https://software.intel.com/en-us/vtune)
  - Stop guessing why software is slow. Advanced sampling and profiling techniques quickly analyze your code, isolate issues, and deliver insights for optimizing performance on modern processors
- NVIDIA DALI [[GitHub]](https://github.com/NVIDIA/DALI)
  - A library containing both highly optimized building blocks and an execution engine for data pre-processing in deep learning applications
- gpushare-scheduler-extender [[GitHub]](https://github.com/HuaizhengZhang/gpushare-scheduler-extender)
  - Some of these tasks can be run on the same Nvidia GPU device to increase GPU utilization
- TensorRT [[NVIDIA]](https://docs.nvidia.com/deeplearning/sdk/tensorrt-developer-guide/index.html)
  - It is designed to work in a complementary fashion with training frameworks such as TensorFlow, Caffe, PyTorch, MXNet, etc. It focuses specifically on running an already trained network quickly and efficiently on a GPU for the purpose of generating a result

## Project

- Weld: Weld is a runtime for improving the performance of data-intensive applications. [[Project Website]](https://www.weld.rs/)
- MindsDB: MindsDB's goal is to make it very simple for developers to use the power of artificial neural networks in their projects [[GitHub]](https://github.com/mindsdb/mindsdb)
- PAI: OpenPAI is an open source platform that provides complete AI model training and resource management capabilities. [[Microsoft Project]](https://github.com/Microsoft/pai#resources)
- Bistro: Scheduling Data-Parallel Jobs Against Live Production Systems [[Facebook Project]](https://github.com/facebook/bistro)
- Osquery is a SQL powered operating system instrumentation, monitoring, and analytics framework. [[Facebook Project]](https://osquery.io/)
- TVM: An Automated End-to-End Optimizing Compiler for Deep Learning
[[Project Website]](https://tvm.ai/)
- Horovod: Distributed training framework for TensorFlow, Keras, and PyTorch. 
[[GitHub]](https://github.com/uber/horovod)
- Seldon: Sheldon Core is an open source platform for deploying machine learning models on a Kubernetes cluster.[[GitHub]](https://github.com/SeldonIO/seldon-core)
- Kubeflow: Kubeflow is a machine learning (ML) toolkit that is dedicated to making deployments of ML workflows on Kubernetes simple, portable, and scalable. [[GitHub]](https://github.com/kubeflow/pipelines)

  
## Model Deployment Papers

- Clipper: A Low-Latency Online Prediction Serving System [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-crankshaw.pdf)
[[GitHub]](https://github.com/ucbrise/clipper)
  - Crankshaw, Daniel, et al. (*NSDI 2017*)
  - Summary: Adaptive batch 
- InferLine: ML Inference Pipeline Composition Framework [[Paper]](https://arxiv.org/pdf/1812.01776.pdf)
  - Crankshaw, Daniel, et al. (*Preprint*)
  - Summary: update version of Clipper
- TrIMS: Transparent and Isolated Model Sharing for Low Latency Deep LearningInference in Function as a Service Environments [[Paper]](https://arxiv.org/pdf/1811.09732.pdf)
  - Dakkak, Abdul, et al (*Preprint*)
  - Summary: model cold start problem

## Machine Learning System Papers (Inference)

- Dynamic Space-Time Scheduling for GPU Inference [[Paper]](http://learningsys.org/nips18/assets/papers/102CameraReadySubmissionGPU_Virtualization%20(8).pdf)
  - Jain, Paras, et al. (*NIPS 18, System for ML*)
  - Summary: 
- Dynamic Scheduling For Dynamic Control Flow in Deep Learning Systems [[Paper]](http://www.cs.cmu.edu/~jinlianw/papers/dynamic_scheduling_nips18_sysml.pdf)
  - Wei, Jinliang, Garth Gibson, Vijay Vasudevan, and Eric Xing. (*On going*)
- Accelerating Deep Learning Workloads through Efficient Multi-Model Execution. [[Paper]](https://cs.stanford.edu/~matei/papers/2018/mlsys_hivemind.pdf)
  - D. Narayanan, K. Santhanam, A. Phanishayee and M. Zaharia. (*NeurIPS Systems for ML Workshop 2018*)
  - Summary: They assume that their system, HiveMind, is given as input models grouped into model batches that are amenable to co-optimization and co-execution. a compiler, and a runtime.

## Machine Learning System Papers (Training)

- Beyond data and model parallelism for deep neural networks [[Paper]](https://arxiv.org/pdf/1807.05358.pdf)
  - Jia, Zhihao, Matei Zaharia, and Alex Aiken. (*SysML 2019*)
  - Summary: SOAP (sample, operation, attribution and parameter) parallelism. Operator graph, device topology and extution optimizer. MCMC search algorithm and excution simulator.
- Device placement optimization with reinforcement learning [[Paper]](https://arxiv.org/pdf/1706.04972.pdf)
  - Mirhoseini, Azalia, Hieu Pham, Quoc V. Le, Benoit Steiner, Rasmus Larsen, Yuefeng Zhou, Naveen Kumar, Mohammad Norouzi, Samy Bengio, and Jeff Dean. (*ICML 17*)
  - Summary: Using REINFORCE learn a device placement policy. Group operations to excute. Need a lot of GPUs.
- Spotlight: Optimizing device placement for training deep neural networks  [[Paper]](http://proceedings.mlr.press/v80/gao18a/gao18a.pdf)
  - Gao, Yuanxiang, Li Chen, and Baochun Li (*ICML 18*)
- GPipe: Efficient Training of Giant Neural Networks using Pipeline Parallelism [[Paper]](https://arxiv.org/pdf/1811.06965.pdf)[[GitHub]](https://github.com/tensorflow/lingvo/blob/master/lingvo/core/gpipe.py) [[News]](https://www.cnbeta.com/articles/tech/824495.htm)
  - Huang, Yanping, et al. (*arXiv preprint arXiv:1811.06965 (2018)*)
  - Summary: 
  
## Resource Management

- Resource management with deep reinforcement learning [[Paper]](https://people.csail.mit.edu/alizadeh/papers/deeprm-hotnets16.pdf) [[GitHub]](https://github.com/hongzimao/deeprm)
  - Mao, Hongzi, Mohammad Alizadeh, Ishai Menache, and Srikanth Kandula (*ACM HotNets 2016*)
  - Summary:  Highly cited paper. Nice definaton. An example solution that translates the problem of packing tasks with multiple resource demands into a learning problem and then used DRL to solve it.
  
## Deep Reinforcement Learning System

- Ray: A Distributed Framework for Emerging {AI} Applications [[GitHub]](https://www.usenix.org/conference/osdi18/presentation/moritz)
  - Moritz, Philipp, et al. (*OSDI 2018*)
  - Summary: Distributed DRL training, simulation and inference system. Can be used as a high-performance python framework.

## Video System papers

- Live Video Analytics at Scale with Approximation and Delay-Tolerance [[Paper]](https://www.microsoft.com/en-us/research/wp-content/uploads/2017/02/videostorm_nsdi17.pdf)
  - Zhang, Haoyu, Ganesh Ananthanarayanan, Peter Bodik, Matthai Philipose, Paramvir Bahl, and Michael J. Freedman. (*NSDI 2017*)
- Chameleon: scalable adaptation of video analytics [[Paper]](http://people.cs.uchicago.edu/~junchenj/docs/Chameleon_SIGCOMM_CameraReady.pdf)
  - Jiang, Junchen, et al. (*SIGCOMM 2018*)
  - Summary: Configuration controller for balancing accuracy and resource. Golden configuration is a good design. Periodic profiling often exceeded any resource savings gained by adapting the configurations.

## Edge or Mobile Papers 

- NestDNN: Resource-Aware Multi-Tenant On-Device Deep Learning for Continuous Mobile Vision [[Paper]]()
  - Fang, Biyi, Xiao Zeng, and Mi Zhang. (*MobiCom 2018*)
  - Summary: Borrow some ideas from network prune. The pruned model then recovers to trade-off computation resource and accuracy at runtime
- Lavea: Latency-aware video analytics on edge computing platform [[Paper]](http://www.cs.wayne.edu/~weisong/papers/yi17-LAVEA.pdf)
  - Yi, Shanhe, et al. (*Second ACM/IEEE Symposium on Edge Computing. ACM, 2017.*)

## Advanced Theory

- Differentiable MPC for End-to-end Planning and Control [[Paper]](https://www.cc.gatech.edu/~bboots3/files/DMPC.pdf)  [[GitHub]](https://locuslab.github.io/mpc.pytorch/)
  - Amos, Brandon, Ivan Jimenez, Jacob Sacks, Byron Boots, and J. Zico Kolter (*NIPS 2018*)
  
## Traditional System Optimization Papers

- AutoScale: Dynamic, Robust Capacity Management for Multi-Tier Data Centers
[[Paper]](https://www3.cs.stonybrook.edu/~anshul/tocs12.pdf)
- Gandhi, Anshul, et al. (*TOCS 2012*)

