# Project Name Here
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:
```HTML 
<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site -->
```

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Dhruv K | Liberty High School | Computer Science | Incoming Junior

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# Final Milestone


<iframe width="560" height="315" src="https://www.youtube.com/embed/ychKdbRGAEc?si=CUknFtZ69xeNqoUM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
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

# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```


# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
