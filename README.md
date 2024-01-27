# Vezir.AI
Vezir.ai employs the method of reinforcement learning to develop a model capable of learning and playing chess. The fundamental objective of the project is to enable an AI model, initially devoid of any knowledge about the game, to comprehend and engage in chess starting from the ground up.

![](https://github.com/asametyildirim/vezirai/blob/main/images/vezir-ai.png)

I won't release the project's code as open-source until a stable model has been developed, as I am endeavoring to create a core model on my own and do not wish to receive assistance during this process. However, I will share the games played by Vezir.ai here with every update. :)

### Third Day:
<table>
<tr>
<td>

![]()

</td>
<td>

- n_steps = 
- Iterations = 
- loss = 
- value_loss = 
- policy_gradient_loss = 
- entropy_loss = 

</td>
</tr>
</table>
**Note:** 


### Day Second:
<table>
<tr>
<td>

![](https://github.com/asametyildirim/vezirai/blob/main/images/vezirai_game2.gif)

</td>
<td>

- n_steps = 49152
- Iterations = 30
- loss = 7.63e-06  
- value_loss = 5.81
- policy_gradient_loss = 0.0466
- entropy_loss = -2.68

</td>
</tr>
</table>
**Note:** It was discovered that during the training phase of vezir.ai, it played both its own side and the opposing side. It will only play its own color, while the opponent was updated to make random moves. Initially, I want it to be able to find at least the legal moves. Moreover, it was determined that the n_steps parameter, set at 2048, was insufficient for finding the legal moves. The value of the n_steps parameter was updated to 49152, giving vezir.ai more time to learn. We observe improvements at the beginning of the chess game, but it still takes too long to find legal moves. It appears that it's not learning the legal moves well. Additionally, it seems that having the opponent make random moves during training is causing it to make random moves as well.

### Day One:
<table>
<tr>
<td>

![](https://github.com/asametyildirim/vezirai/blob/main/images/vezirai_game1.gif)

</td>
<td>

- n_steps = 2048
- Iterations = 450
- loss = 1.21e+04
- value_loss = 2.5e+04
- policy_gradient_loss = -0.0047
- entropy_loss = -8.32

</td>
</tr>
</table>
**Note:** It appears to be attempting invalid moves at least 300 times before each actual move. It seems like it hasn't learned how the pieces move or grasped the rules of chess..


