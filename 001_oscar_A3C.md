# Asynchronous Methods for Deep Reinforcement Learning

Mock-up

The authors propose an asynchronous optimization method, wich work on four standard reinforcement learning algorithm:

- SARSA ()
- one-step DQN
- n-step DQN (with forward view)
- Advantage Actor Critic (They called it A2C, but the idea came from the REINFORCE algorithm).

*It is called advantage because the weight (as in spinning up indicate) is estimated with the advantage.

NOTE: Worthed to put notes about that too.

*REINFORCE is the vanilla policy gradient method more general case, where you can use any kind of b, or event don't use advantage.


- They address the problem of non-stationary and correlated RL updates by asynchronously updating some global parameters by multiple agents, which have their own copy of the environment.
- How the parallel actor maximimze diversity and allow a more stable update. Why experience replay can be omited (but it could be useful afterall)
- It is called A3C because it includes the Asyncronous to A2C
- Talk about batch learning
- The forward view of the rollout (an there exist other)
- Why is called actor and critic

TAKE A foto the main algorithm a put it here


Open question
- SARSA is an on-policy or off-policy methods, and why?
- What is the relation between target and behavior parameters when talking about on-policy and off-policy?
- What is the backward view?
- How they calculate the entropy and why is useful?