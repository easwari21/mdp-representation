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

-1  --> If the agent makes any invalid move. 

### Graphical Representation

<img width="1600" height="1321" alt="WhatsApp Image 2026-04-24 at 4 16 04 PM" src="https://github.com/user-attachments/assets/1f2b4419-c002-4baa-b9fe-6701b8883a37" />


## PYTHON REPRESENTATION:
```
P = {
    1:{
        0: [(0.5,1,0,True)],
        1: [(0.5,2,1,True)]
    },
    2:{
        0: [(0.5,1,1,True)],
        1: [(0.5,3,1,True)]
    },
    3:{
        0: [(0.5,2,1,True)],
        1: [(0.5,4,10,True)]
    }
    4:{
        0: [(0.5,3,1,True)],
        1: [(0.5,4,-1,True)]
    }
}


```

## OUTPUT:
Write your Python output here

## RESULT:
Thus a real world problem has successfuly explained through MDP Process.

