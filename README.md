# MDP REPRESENTATION

## AIM:
To represent a real world Reinforcement Learning based problem using MDP Representation.

## PROBLEM STATEMENT:
A Pathway in a field where the agent can move forward or backward to reach the terminal state and obtain reward.

### Problem Description
The limited space Pathway in a rice field  has 4 States where the agent have to move forward or backward to reach the final state,If the agent manages to reach the terminal state it earns a certain amount of points.The goal is to navigate the agent to reach the goal state by offering reward points.

### State Space

States- [1, 2, 3, 4]

### Sample State

Sample state is State 2.

### Action Space

There are two actions that can be performed:

1.Moving forward

2.Moving backward

### Sample Action

Moving Forward

### Reward Function

+10 --> If the agent reaches the Terminal State.

+1  --> If the agent moves forward to any state that is not Terminal State.

 0  --> If the agent moves backward to any state that is not Terminal State.


### Graphical Representation

<img width="1600" height="941" alt="WhatsApp Image 2026-04-24 at 10 21 06 PM" src="https://github.com/user-attachments/assets/dfb4da28-8058-4e6b-b24d-ac163de45b8d" />



## PYTHON REPRESENTATION:
```
P = {
    1: {
        0: [(0.8, 1, 0, False), (0.2, 1, 0, False)],  
        1: [(0.8, 2, 1, False), (0.2, 1, 0, False)]    
    },

    2: {
        0: [(0.8, 1, 0, False), (0.2, 2, 0, False)],  
        1: [(0.8, 3, 1, False), (0.2, 2, 0, False)]    
    },

    3: {
        0: [(0.8, 2, 0, False), (0.2, 3, 0, False)],   
        1: [(0.8, 4, 10, True), (0.2, 3, 0, False)]    
    },

    4: {
        0: [(1.0, 4, 0, True)],   
        1: [(1.0, 4, 0, True)]
    }
}
```

## OUTPUT:

<img width="626" height="162" alt="image" src="https://github.com/user-attachments/assets/acf9c536-fae2-471e-88f5-9063c0b000c7" />


## RESULT:
Thus a real world problem has successfuly explained through MDP Process.

