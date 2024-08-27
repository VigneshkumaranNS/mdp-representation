# MDP REPRESENTATION

## AIM:
The representation of real world scenario using Markov Decision Process by stating all the states,actions and environment with respective rewards.

## PROBLEM STATEMENT:
~~~
By: Vignesh Kumaran N S
RegNo: 212222230171
~~~

### Problem Description
Developing an environment in a room where there is a temperature control system which acts as an agent to maintain the temperature between extreme cold, cold and comfort.
The goal of the agent is to maintain the temperature always at the comfort.

### State Space
{1,0,2} -{Comfort, Cold, Extreme Cold}

### Sample State
1 {Comfort}
### Action Space
{0,1,2} ={Maintain Temperature, Increase Temperature, Decrease Temperature}

### Sample Action
1 {Increase Temperature}

### Reward Function
+1 if reached the comfort.
0 Other wise.

### Graphical Representation

<img width="1353" alt="image" src="https://github.com/KoduruSanathKumarReddy/mdp-representation/assets/69503902/45528046-c646-4479-ba92-a94aafa0e255">



## PYTHON REPRESENTATION:
~~~
temperature ={
    0:{
        0:[(0.7,0,0.0,False),(0.2,1,1.0,True),(0.1,2,0,True)],
        1:[(0.7,1,1.0,True),(0.2,2,0.0,True),(0.1,0,0,False)],
        2:[(0.7,2,0.0,True),(0.2,1,1.0,True),(0.1,0,0,False)]

    },
    1:{
        0:[(0.7,1,1.1,True),(0.2,1,1.0,True),(0.1,0,0.0,False)],
        1:[(0.7,1,1,1,True),(0.2,0,0.0,False),(0.1,1,1.0,True)],
        2:[(0.7,0,0.0,False),(0.2,1,1.0,True),(0.1,1,1.0,True)]
    },
    2:{
        0:[(0.7,2,0.0,True),(0.2,0,0.0,False),(0.1,2,0.0,True)],
        1:[(0.7,0,0.0,False),(0.2,2,0.0,True),(0.1,2,0.0,True)],
        2:[(0.7,2,0.0,True),(0.2,0,0.0,False),(0.1,2,0.0,False)]

    }

}
~~~

## OUTPUT:
<img width="648" alt="image" src="https://github.com/KoduruSanathKumarReddy/mdp-representation/assets/69503902/c8de9300-afc1-4640-a045-7c5292f713a2">


## RESULT:
Therefore an MDP representation has been created for a real world scenario with all the states, actions and rewards.

