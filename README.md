# Optimized-Task-Scheduling
Optimized task scheduling refers to the process of efficiently allocating computational tasks to available computing resources to achieve specific objectives such as minimizing makespan (the total time taken to complete all tasks), maximizing resource utilization, meeting deadlines, or minimizing energy consumption. 

## About
Task scheduling is the process of allocating tasks to the VMs (Virtual Machines). It can be optimized using certain algorithms. Many cloud platforms can be used on which you can perform optimization. This is a research-based project which is performed by __"Perfect Cube"__ (my team). We used a cloud simulator named __"CloudSim"__ for conducting this research. For optimizing the process of Task scheduling, We have used Reinforcement Learning techniques like Q-Learning and SARSA;  and also used some existing algorithms like Whale Optimization Algorithm, Genetic Algorithm, Hybrid Whale Genetic Algorithm, etc and combined them with Q Learning and SARSA.

## Q Learning
Task scheduling using Q-learning is a reinforcement learning approach to solve the problem of scheduling tasks on computing resources efficiently. In this context, tasks can represent various computational jobs or processes, and computing resources can include CPUs, GPUs, or other types of hardware.

Q-learning is a model-free reinforcement learning technique where an agent learns to make decisions by interacting with an environment to maximize a cumulative reward. In the context of task scheduling, the agent is responsible for deciding which tasks to assign to which computing resources at any given time.

By employing Q-learning for task scheduling, it's possible to optimize resource allocation in dynamic and complex computing environments, leading to improved efficiency and better utilization of resources.

## SARSA
SARSA (State-Action-Reward-State-Action) is another reinforcement learning algorithm that can be applied to task scheduling problems. Using SARSA for task scheduling allows for the optimization of resource allocation in dynamic and complex computing environments, leading to improved efficiency and better utilization of resources, similar to Q-learning. SARSA is particularly well-suited for scenarios where the agent needs to interact with the environment in real-time, making it a potentially suitable choice for online task scheduling problems.

In Q Learning, where we are using this formula,
![](https://miro.medium.com/v2/resize:fit:1043/1*vTMQI14ls9lWzRXzJGi4sg.jpeg)
We will use this formula in SARSA, 
![](https://miro.medium.com/v2/resize:fit:1400/1*cXlwV7vlOhQUZiATkmln3A.png)

In SARSA, instead of selecting maximum valued action like in Q Learning, we use epsilon greedy policy to select action.

## Whale Optimzation Algorithm
