The project uses wandb to run a pipeline of transformers. 

First I import the required libraries, then I initialie wandb using wandb API key.

I have kept the key in another environment file forconfidentiality purpose.

Then I set my data mode to test = False

If API key or dataset is not provided, set the error to inform user.

I used a small training set 'bert-tiny-training' from hugging face. 

I loaded dataset and divided into training and test data. 

For timeutilization , i filter data tochoose only a small portion of training and test data.

I set the tokenizer, and encode the train and test data using tokenizer.

I trained model and set evaluation metrics. I set training arguments. 

It is necessary to set report_to='wandb' so that logs and artifacts are kept in wandb.

I initialize the training model and save mymodel results in wandb.
