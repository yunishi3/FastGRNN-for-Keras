# EdgeML FastGRNN/FastRNN cells for Keras

This repository is FastGRNN and FastRNN cells for Keras implementation. This is just a little modified from the original tensorflow implementation as follows.  
[https://github.com/microsoft/EdgeML](https://github.com/microsoft/EdgeML)  
  
The original code license is as follows. Sincerely respect for the original code.  
  
Copyright (c) Microsoft Corporation. All rights reserved.  
Licensed under the MIT license.
  
  
Original Paper is here.  
[FastGRNN: A Fast, Accurate, Stable and Tiny Kilobyte Sized Gated Recurrent Neural Network](https://arxiv.org/abs/1901.02358)  
  
  
## FastGRNN/FastRNN cells for Keras
This is almost copied from "EdgeML/examples/tf/FastCells"  
And rnn.py is moved from "EdgeML/tf/edgeml_tf/graph.rnn.py"  
FastGRNN and FastRNN cells for Keras are included in rnn.py.  
  
Modified codes are 2 files in this directory as follows.  
#### rnn.py  
I just added  
`def gen_non_linearity_keras`  
`class FastGRNNCellKeras(RNNCell)`  
`class FastRNNCellKeras(RNNCell)`    
for Keras implementation.
  

#### fastcell\_example\_keras.ipynb  
You can refer this example notebook to implement FastGRNN/FastRNN cells to your code. This example code is also taken from the original [fastcell_example.ipynb](https://github.com/microsoft/EdgeML/blob/master/examples/tf/FastCells/fastcell_example.ipynb).  The network model and training code were modified for Keras.  
  
I think this repository might work since the training results were similar with the original tensorflow version.  
  
  
##### -Note:This implementation doesn't support training to induce sparsity.
  
The other details are in [the original explanation](https://github.com/microsoft/EdgeML/tree/master/examples/tf/FastCells).  
  
Thanks!!