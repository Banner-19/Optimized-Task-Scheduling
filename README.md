# Optimized-Task-Scheduling
Optimized task scheduling refers to the process of efficiently allocating computational tasks to available computing resources to achieve specific objectives such as minimizing makespan (the total time taken to complete all tasks), maximizing resource utilization, meeting deadlines, or minimizing energy consumption. 

## About
Task scheduling is the process of allocating tasks to the VMs (Virtual Machines). It can be optimized using certain algorithms. Many cloud platforms can be used on which you can perform optimization. This is a research-based project which is performed by __"Perfect Cube"__ (my team). We used a cloud simulator named __"CloudSim"__ for conducting this research. For optimizing the process of Task scheduling, We have used Reinforcement Learning techniques like Q-Learning and SARSA;  and also used some existing algorithms like Whale Optimization Algorithm, Genetic Algorithm, Hybrid Whale Genetic Algorithm, etc and combined them with Q Learning and SARSA.

## Q Learning
Task scheduling using Q-learning is a reinforcement learning approach to solve the problem of scheduling tasks on computing resources efficiently. In this context, tasks can represent various computational jobs or processes, and computing resources can include CPUs, GPUs, or other types of hardware.

Q-learning is a model-free reinforcement learning technique where an agent learns to make decisions by interacting with an environment to maximize a cumulative reward. In the context of task scheduling, the agent is responsible for deciding which tasks to assign to which computing resources at any given time.

By employing Q-learning for task scheduling, it's possible to optimize resource allocation in dynamic and complex computing environments, leading to improved efficiency and better utilization of resources.

[Reference](https://www.techtarget.com/searchenterpriseai/definition/Q-learning#:~:text=Q%2Dlearning%20is%20a%20machine,way%20animals%20or%20children%20learn.)

## SARSA
SARSA (State-Action-Reward-State-Action) is another reinforcement learning algorithm that can be applied to task scheduling problems. Using SARSA for task scheduling allows for the optimization of resource allocation in dynamic and complex computing environments, leading to improved efficiency and better utilization of resources, similar to Q-learning. SARSA is particularly well-suited for scenarios where the agent needs to interact with the environment in real-time, making it a potentially suitable choice for online task scheduling problems.

In Q Learning, where we are using this formula,
![](https://miro.medium.com/v2/resize:fit:1043/1*vTMQI14ls9lWzRXzJGi4sg.jpeg)
We will use this formula in SARSA, 
![](https://miro.medium.com/v2/resize:fit:1400/1*cXlwV7vlOhQUZiATkmln3A.png)

In SARSA, instead of selecting maximum valued action like in Q Learning, we use epsilon greedy policy to select action.

[Reference](https://www.geeksforgeeks.org/sarsa-reinforcement-learning/)

## Whale Optimzation Algorithm
Whale optimization algorithm (WOA): A nature inspired meta-heuristic optimization algorithm which mimics the hunting behaviour of humpback whales. The algorithm is inspired by the bubble-net hunting strategy  

Foraging behavior of Humpback whales is called bubble-net feeding method. Humpback whales prefer to hunt school of krill or small fishes close to the surface. It has been observed that this foraging is done by creating distinctive bubbles along a circle or ‘9’-shaped path 

Bubble-net feeding is a unique behaviour that can only be observed in humpback whales. In whale optimization algorithm (WOA) the spiral bubble-net feeding maneuver is mathematically modeled in order to perform optimization

* WOA simulated hunting behaviour with random or the best search agent to chase the prey
* WOA uses a spiral to simulate bubble-net attacking mechanism of humpback whales

[Reference](https://www.geeksforgeeks.org/whale-optimization-algorithm-woa/)

## Genetic Algorithm
Genetic Algorithms(GAs) are adaptive heuristic search algorithms that belong to the larger part of evolutionary algorithms. Genetic algorithms are based on the ideas of natural selection and genetics. These are intelligent exploitation of random searches provided with historical data to direct the search into the region of better performance in solution space.

Genetic algorithms are based on an analogy with the genetic structure and behavior of chromosomes of the population. Following is the foundation of GAs based on this analogy –  

* Individuals in the population compete for resources and mate
* Those individuals who are successful (fittest) then mate to create more offspring than others
* Genes from the “fittest” parent propagate throughout the generation, that is sometimes parents create offspring which is better than either parent.
* Thus each successive generation is more suited for their environment.

[Reference](https://www.geeksforgeeks.org/genetic-algorithms/)

## Hybrid Whale Q Learning Algorithm
Hybridizing Whale Optimization Algorithm (WOA) with Q-learning can offer a robust approach to task scheduling in dynamic and complex computing environments. 

The Q-learning component continuously learns from the performance of the WOA-generated solutions by updating Q-values based on the observed rewards.
These updated Q-values influence the behavior of the WOA component in subsequent iterations, guiding it towards regions of the search space associated with higher rewards.

By combining the strengths of both WOA and Q-learning, the hybrid approach can effectively address the task scheduling problem in dynamic and complex computing environments, offering improved efficiency and resource utilization.

## Hybrid Whale SARSA Algorithm
In a hybrid approach that combines the Whale Optimization Algorithm (WOA) with SARSA (State-Action-Reward-State-Action), the Whale Optimization Algorithm is employed to generate candidate solutions for task scheduling, while SARSA guides the exploration process by providing feedback on solution quality. 

In the hybrid approach, the WOA component generates candidate solutions for task scheduling.
These solutions are evaluated based on their quality, which may include factors such as makespan, resource utilization, and deadline adherence.
SARSA is then used to guide the exploration process of WOA by providing feedback on the quality of generated solutions.
SARSA's learned policy can influence the selection of actions (solutions) generated by WOA, biasing it towards regions of the solution space associated with higher rewards

The hybrid approach leverages WOA's optimization capabilities and SARSA's reinforcement learning framework.
Addresses task scheduling challenges in dynamic environments, leading to improved efficiency and resource utilization.
