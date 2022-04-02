# Colossalai
Colossalai is a distributed training framework developed by Prof Yang
You’s team
Learning rate range test is a method proposed by Leslie N. Smith in paper Super-Convergence: Very Fast Training of Neural Networks Using Large Learning Rates. The idea is: before normally training your model to convergence, first train your model with exponentially increasing learning rate (increase with batch step) for several epochs, and observe the loss curve. 
Usually the loss will first keep unchanged, and then go down, and finally explode. The learning rate corresponding to loss going down will be usable LR, and explosion part is not usable. 
Depending on your chosen optimizer and learning rate scheduling, this method can give you reference for LR choice region, and for some of the settings this method can serve as a super fast tuning method with high performance.
