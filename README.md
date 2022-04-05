# Continuous-Environment

Here are presented two algorithms that work in continuous enviroments:       
*DDPG : https://spinningup.openai.com/en/latest/algorithms/ddpg.html            
*TD3: https://spinningup.openai.com/en/latest/algorithms/td3.html                      

In 'main_function' we can change parameters to train some Agents with different configurations.           
Here are some training results:

![bla1](https://user-images.githubusercontent.com/102504166/161746725-43930f06-ae6f-4406-acc9-7beaaf8bccc2.png)
![bla2](https://user-images.githubusercontent.com/102504166/161746729-3d367845-bcc1-49b7-95bd-efbb624aadb8.png)
![bla3](https://user-images.githubusercontent.com/102504166/161746731-ebbfb6ee-6a74-433d-95dc-07964875e2d8.png)

Configuration:                                
Agent1_DDPG (hidden_l1 =250, hidden_l1 =250, actor_lr =1e-4, critic_lr =1e-3, gamma =0.99, tau =1e-2, memory_size =50000,  num_of_hd_layers =2)                   
Agent2_DDPG (hidden_l1 =350, hidden_l1 =350, actor_lr =1e-4, critic_lr =1e-3, gamma =0.99, tau =1e-2, memory_size =50000,  num_of_hd_layers =2)                        
Agent3_TD3 (hidden_l1 =350, hidden_l1 =350, actor_lr =1e-4, critic_lr =1e-3, gamma =0.99, tau =1e-2, memory_size =50000,  num_of_hd_layers =2, popicy_delay =2)                 

The 'train()' method can return the average rewards and we can store it in some variables. Thus we can train multiple Agents with different parameters and compare their evolutions.                     
![bla4](https://user-images.githubusercontent.com/102504166/161748228-a82ecd02-7d63-4479-ac60-542ba8b5a7f6.png)
