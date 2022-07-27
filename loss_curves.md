# Loss curves explanation

We can find a multiple types of loss curves, and each one has some specific details that can be related to some patterns.

In the next images we're going to see some examples and its possible explanation.

---

![1](img/1.png)

- Here we can see that our validation loss is **lower**  than training loss.
- It usually indicates that the training data is harder to model than the validation data, and **the model may not be good enough.**
- It's possible to think about an improperly splitting of the data. The randomness in the splitting can avoid to show some data in our training phase and it can hide details to the model.
- Different splittings can return different results on the training, because the model is seeing different examples each time.

![dropout](img/dropout.png)

- Here we can see a simple model, because the validation loss is lower than the training loss
- Here with the dropout during the training, a percentage of features are set to zero. During the testing all neurons are used. So the model during the training is more robust, and can lead to higher testing acurracies.
- In other words, for training it makes it harder than in testing.
- The value for dropout 0.2 or 0.5 means that during the training phase 20% or 50% percentage of neurons are going to be disabled, So during the testing is more robust.

