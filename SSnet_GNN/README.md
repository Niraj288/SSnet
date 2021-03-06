

## Usage

We provide two major scripts:

- code/preprocess_data.py creates the input tensor data of CPIs
for processing with PyTorch from the original data
(see gen_dude/original/data.txt). To create your own make a directory and place the data as name_of_data/original/data.txt (make sure to change dataset name in preprocessing.sh)
- code/run_training.py trains the model using the above preprocessed data
(make sure to change dataset name in run_training.sh).

(i) Create the tensor data of CPIs with the following command:
```
cd code
bash preprocess_data.sh
```

The preprocessed data are saved in the dataset/input directory.

(ii) Using the preprocessed data, train the model with the following command:
```
bash run_training.sh
```

The training and test results and the model are saved in the output directory
(after training, see output/result and output/model).

(iii) You can change the hyperparameters in preprocess_data.sh and run_training.sh.
Try to learn various models.
