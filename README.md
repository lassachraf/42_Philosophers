# Philosophers Project

![](https://camo.githubusercontent.com/026f17ed41fee573861aef3ca619febc8c9f00f3c495a7200026957acdb9686d/68747470733a2f2f6d656469612e6c6963646e2e636f6d2f646d732f696d6167652f4435363132415147364648334831306e6971672f61727469636c652d636f7665725f696d6167652d736872696e6b5f3732305f313238302f302f313639303639383239323335383f653d3231343734383336343726763d6265746126743d416a324644746a574a35316361455878362d4a564c4b5f773975673265626b4677654e73526478694c5163)

# Introduction

The "Philosophers" project is part of the 42 Network's Common Core curriculum. It revolves around the famous "Dining Philosophers" problem, which is a classic synchronization issue in computer science used to illustrate the challenges of resource sharing and concurrency.

# Project Overview

### Objective:
The project aims to train students in multi-threading and multi-process programming using mutexes and semaphores. It involves implementing simulations of the Dining Philosophers problem with different synchronization techniques.

### Key Concepts:

  **Dining Philosophers Problem:**
      * Philosophers sit at a circular table with a bowl of spaghetti and a fork between each pair.
      * Each philosopher must alternate between eating, thinking, and sleeping.
      * To eat, a philosopher needs two forks, which introduces a challenge to avoid deadlock and 
      ensure no philosopher starves.

  **Project Variants:**
      * **Mandatory part :** Uses multi-threading with mutexes.
      * **Bonus part :** Uses multi-processing with semaphores.

### Rules and Requirements:

  * The simulation must ensure that no philosopher starves.
  * Philosophers do not communicate with each other.
  * The simulation stops when a philosopher dies of starvation.
  * The project must be coded in C, adhering to the 42 Norm, which 
    includes strict coding standards and no memory leaks or crashes.

### Compilation and Execution

```bash
git clone https://github.com/lassachraf/42_Philosophers.git
```
```bash
cd 42_Philosophers
```
* For mandatory :
``` bash
make
```
``` bash
./philo nb_philo time_to_die time_to_eat time_to_sleep max_meals
```
* For bonus :
``` bash
make bonus
```
``` bash
./philo_bonus nb_philo time_to_die time_to_eat time_to_sleep max_meals
```
  * nb_philo : Number of philosophers.
  * time_to_die : Time to die in milliseconds.
  * time_to_eat : Time to eat in milliseconds.
  * time_to_sleep : Time to sleep in milliseconds.
  * max_meals : Number of times each philosopher must eat (Optional parameter).

# Learning Outcomes

   * Managing concurrency and synchronization in software development.
   * Using mutexes and semaphores to handle shared resources.
   * Optimizing C code for performance, which is critical for real-time systems.

