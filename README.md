# TRANSFORMERS
Building transformer model from scratch. Creating layers and finally combining all to make transformer model.

<img src="transformer.png" alt="Transformer" width="550"></img>

<caption><center><font color='purple'><b>Figure: Transformer</b></font></center></caption>
<br>
<br>
The flow of data through the Transformer Architecture is as follows:

* First your input passes through an Encoder, which is just repeated Encoder layers that you implemented:
    - embedding and positional encoding of your input
    - multi-head attention on your input
    - feed forward neural network to help detect features
* Then the predicted output passes through a Decoder, consisting of the decoder layers that you implemented:
    - embedding and positional encoding of the output
    - multi-head attention on your generated output
    - multi-head attention with the Q from the first multi-head attention layer and the K and V from the Encoder
    - a feed forward neural network to help detect features
* Finally, after the Nth Decoder layer, two dense layers and a softmax are applied to generate prediction for the next output in your sequence.

Encoder and Decoder layers are built first and then combined to form transformer model.
 
The code is accompanied by detailed explanations and illustrations to help you understand how Transformer models work and how to implement them. This repository is ideal for anyone who is interested in Natural Language Processing and wants to learn how to build state-of-the-art models from scratch.
