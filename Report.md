# Report

## Descritpion of the learning algorithm

The algorithm implemented to train the agent is [DDPG](https://arxiv.org/abs/1509.02971).

#### Hyperparameters chosen

- minibatch size: 1024
- replay memory size: 1000000
- discount factor gamma: 0.99
- min squared gradient tau: 0.001
- learning rate actor: 0.00153
- learning rate critic: 0.00103
- weight decay: 0

#### Model Architecture

1. The input to the neural network consists of a 33 x 1 vector including the position, rotation, velocity and angular velocities of the arm

2. The first hidden layer is fully-connected and consists of 400 rectifier units.

3. The second hidden layer is fully-connected and consists of 300 rectifier units.

4. The output layer is a fully-connected linear layer with a single output for each of the 4 valid actions. The output layer uses tanh as output function.

## Performance of the trained agent
The environment is considered solved when the agent gets an average score of *+30* over 100 consecutive episodes, and over all agents.
The agent solved the environment in a total of **251** episodes.

**Trained agent**

![trained_agent](https://user-images.githubusercontent.com/36470989/62230382-f90dc500-b3c1-11e9-9692-43c08819c691.gif)



**Plot of the rewards obtained by the agent during the training**

![reward_plot](https://user-images.githubusercontent.com/36470989/62543155-92732600-b85d-11e9-9825-161c413ed318.png)

## Future improvements

To improve the performance of the agent some of the suggestions for future work are:
- implementation of [PPO](https://blog.openai.com/openai-baselines-ppo/)
- implementation of [D4PG](https://openreview.net/forum?id=SyZipzbCb)
