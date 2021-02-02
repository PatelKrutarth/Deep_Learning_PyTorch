#### Image_Classification_Parameter_Tuning
- Using PyTorch with three different levels of abstraction.
 - Part I, Preparation: we will use CIFAR-10 dataset.
 - Part II, Barebones PyTorch: Abstraction level 1, we will work directly with the lowest-level PyTorch Tensors.
 - Part III, PyTorch Module API: Abstraction level 2, we will use nn.Module to define arbitrary neural network architectures.
  - Part IV, PyTorch Sequential API: Abstraction level 3, we will use nn.Sequential to define a linear feed-forward network very conveniently.
 - Part V, Tuning: Experiment with different architectures, activation functions, weight initializations, optimizers, hyperparameters, regularizations or other advanced features.

#### Sentiment_Classification
- Implementation of RNN, and LSTM based sentiment classifiers using word level input. The last hidden state is used as a sentense respresentation for the classification task.
- Also experimented with Bidirectional-LSTM network.
- Used GloVe 300d embeddings trained on Wikipedia 2014 \+ Gigaword 5 (glove.6B.zip) available at https://nlp.stanford.edu/projects/glove/.
- The Stanford Sentiment Treebank (SST-5) dataset is used for train/validation/test. Provided in the directory.

#### Disaster_Image_Classification_Finetuning_pretrained_CNN
- Used pretrained VGG11 Model, finetuned last few layers of the pretrained model.
- The dataset is available at https://crisisnlp.qcri.org/#resource9. Train/validation/test subsets are provided for each event in the dataset. In the original dataset, there are three damage classes: severe, mild, and none. However, Nguyen et al. (2017) suggested that the task of discriminating between mild and severe damage is very subjective, and there is significant overlap in the dataset between the two classes. Therefore, severe and mild classes are combined into one class called damage.