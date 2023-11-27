# [NeurIPS Citylearn Challenge](https://www.aicrowd.com/challenges/neurips-2022-citylearn-challenge)


This repository contains the project for the Collaborative AI class which was to find solution for the NeurIPS  Citylearn Challenge.

#  Competition Overview
[The CityLearn Challenge 2022](https://www.aicrowd.com/challenges/neurips-2022-citylearn-challenge) focuses on the opportunity brought on by home battery storage devices and photovoltaics. It leverages [CityLearn](https://github.com/intelligent-environments-lab/CityLearn/tree/citylearn_2022), a Gym Environment for building distributed energy resource management and demand response. The challenge utilizes 1 year of operational electricity demand and PV generation data from 17 single-family buildings in the Sierra Crest home development in Fontana, California, that were studied for _Grid integration of zero net energy communities_.

Participants will develop energy management agent(s) and their reward function for battery charge and discharge control in each building with the goals of minimizing the monetary cost of electricity drawn from the grid, and the CO<sub>2</sub> emissions when electricity demand is satisfied by the grid.

# Solution Overview


## Phase 1
In the single-agent scenario, we have used the DDPG algorithm . Deep Deterministic Policy Gradient
(DDPG) is an off-policy algorithm particularly well-suited for problems with continuous action spaces. It
aims to concurrently learn an action-value function (Q-function) and a policy function.

## Phase 2 
For the centralized multi-agent scenario, we extend the DDPG framework [3]to create a centralized agent
that manages multiple sub-agents. This centralized agent receives a global state and determines a joint
action, which is then disseminated to each of the sub-agents.

##Phase 3
In the decentralized multi-agent scenario, we propose a hybrid approach that incorporates elements of both
local and global decision-making. This approach utilizes a Deep Implicit Communication Network [4] that
includes a Graph Convolutional Network (GCN) and a Transformer-based encoder for generating communication signals






