# Reinforcement Learning Lunar Lander
For my Bluestamp Engineering project, I trained an AI using reinforcement learning to autonomously land a spacecraft between the flags in the Lunar Lander environment. I experimented with neural network architectures, learning rates, and different AI models like DQN and A2C, overcoming challenges with training and debugging while learning how AI can improve through repeated experimentation.


| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Dhruv K | Liberty High School | Computer Science | Incoming Junior


![Headstone Image](logo.svg)
  
# Final Milestone


<iframe width="560" height="315" src="https://www.youtube.com/embed/ychKdbRGAEc?si=CUknFtZ69xeNqoUM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


- Implemented A2C (Advantage Actor-Critic) as a new reinforcement learning model and compared it with my optimized DQN from the previous milestone. I looked at differences in training time, reward, landing behavior, and consistency.
- My biggest challenge was getting A2C working correctly after adapting the original DQN project. I had to troubleshoot several coding and training issues, but successfully getting a second model running and being able to compare it with DQN was my biggest accomplishment.
- I learned about reinforcement learning, DQN, A2C, neural networks, learning rates, network architecture, rewards, and model training. I also learned how experimentation and debugging are crucial when developing AI models.
- After Bluestamp, I want to continue learning about AI and machine learning, especially how more advanced reinforcement learning algorithms work. I also hope to build more projects where I can apply these concepts to real-world problems.



# Second Milestone


<iframe width="560" height="315" src="https://www.youtube.com/embed/uMRnftdsukE?si=_tWN1w0DkoGMnwpf" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


- Since my first milestone, I experimented with different neural network architectures and learning rates to improve the Deep Q-Network (DQN). After comparing many combinations, I found that a [128,64] network with a 0.0002 learning rate produced the most consistent results, landing within the flags 90% of the time.
- I was surprised that larger neural networks did not always perform better. Some configurations actually reduced performance, showing that choosing the right network architecture was important. Additionally, it was surprising that learning at a slower rate could be beneficial to the lander, showing that faster isn't always better.
- One of the biggest challenges for me was understanding how each parameter affected the DQN's learning process. By testing one variable at a time and collecting data, I was able to identify a combination that significantly improved landing consistency.
- Before my final milestone, I plan to complete a quick analysis of the results from my second milestone, research different models which could possibly land the lunar spacecraft better, and then compare the DQN with the other model.

# First Milestone


<iframe width="560" height="315" src="https://www.youtube.com/embed/laSNHTE5MEQ?si=Bun4pMeJl9cKVh4z" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


- Trained a Deep Q-Network (DQN) to autonomously land a spacecraft using reinforcement learning. The project combines the Lunar Lander environment, a neural network, and a reward system to teach the AI through many trials.
- Successfully trained a baseline DQN model, then began experimenting with different neural network layouts and learning rates to improve landing performance. Trained it to land within the flags.
- Learning how reinforcement learning differs from traditional programming and understanding how hyperparameters like hidden layers and learning rate affect the AI's behavior. Too much swaying of the lander as it lands.
- Continue testing different parameters, compare performance across experiments, select the best-performing setup of parameters, and create a final demonstration of the trained AI landing smoothly and successfully within the flags at least 90% of the time.


# Code

# Code

### Milestone 1 — Baseline DQN

The provided model started with two neural network layers containing 64 neurons each and a learning rate of 0.001. I halved this learning rate and was able to achieve moderate success in landing the spacecraft between the flags.

```python
nn_layers = [64, 64]
learning_rate = 0.0005
```
### Milestone 2 - Optimized DQN

I tested different neural network configurations and learning rates to improve the lander's landing consistency. My improved configuration used 128 neurons in the first layer, 64 in the second, and a learning rate of 0.0002.

```python
nn_layers = [128, 64]
learning_rate = 0.0002
```
This configuration gave me more consistent landings and was able to land within the flags about 90% of the time during my testing.

### Milestone 3 - New A2C Model

For my final milestone, I implemented A2C (Advantage Actor-Critic) as a new reinforcement learning algorithm. I used a [128, 64] neural network and experimented with additional A2C parameters including the number of steps and exploration coefficient.

```python
nn_layers = [128, 64]

learning_rate = 0.0007
n_steps = 8
ent_coef = 0.0001
```
```python
policy_kwargs = dict(
    activation_fn=torch.nn.ReLU,
    net_arch=nn_layers
)

model = A2C(
    "MlpPolicy",
    train_env,
    policy_kwargs=policy_kwargs,
    learning_rate=learning_rate,
    n_steps=n_steps,
    ent_coef=ent_coef,
    gamma=0.99,
    seed=1,
    verbose=1
)
```
I then compared A2C with my optimized DQN based on training time, reward, landing behavior, and consistency.

# Other Resources
- [Bluestamp Engineering Project Notes](https://docs.google.com/document/d/1IQdQ-L8NkyCQ3FZL1m_efOg_2SS5NsGydz_B3h3kJGY/edit?tab=t.0) — Used for project notes, experimentation, and recording observations throughout the Lunar Lander project.
- [Deep Q-Learning — GeeksforGeeks](https://www.geeksforgeeks.org/deep-learning/deep-q-learning/) — Used to learn about Deep Q-Learning and understand how DQN works.
- [Stable-Baselines3 Documentation](https://stable-baselines3.readthedocs.io/) — Used to understand and implement reinforcement learning algorithms including DQN and A2C.

