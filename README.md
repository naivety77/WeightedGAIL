# Learning to Weight Imperfect Demonstrations

This repository contains the PyTorch code for the paper "Learning to Weight Imperfect Demonstrations" in ICML 2021. Code for Atari experiments can be found in [this repo](https://github.com/naivety77/gail_atari).

## Requirement
 * Python 3.7
 * torch 1.3.1
 * gym 0.15.7
 * mujoco 2.0.2.4
 * numpy 1.16.2
 
## Execute
 * WGAIL
 ```
 python wgail.py --env Ant-v2 --num-epochs 5000 --traj-size 1000 --stage 2
 ```
 * 2IWIL
 ```
 python 2iwil.py --env Ant-v2 --num-epochs 5000 --traj-size 1000 --stage 2
 ```
 * GAIL
 ```
 python gail.py --env Ant-v2 --num-epochs 5000 --traj-size 1000 --stage 2
 ```
 * T-REX
 ```
 python trpo_irl.py --env Ant-v2 --num-epochs 5000 --reward-path 'reward_model/ant_reward_stage2.pth' --stage 2
 ```
The re-implementation of T-REX/D-REX can be found in [SAIL](https://github.com/naivety77/SAIL).

## Acknowledegement
We would like to thank the authors of [2IWIL/IC-GAIL](https://github.com/kristery/Imitation-Learning-from-Imperfect-Demonstration). Our code structure is largely based on their source code.
