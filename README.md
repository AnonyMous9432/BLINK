# BLINK

# Install Packages

```python
  pip3 install flair
```
```python
  pip3 install seqeval
```
# Dataset
Please donwload datasets from our paper and save in the data folder

# Training
Run the following code to train the model

```python
  !python3 train.py --dataset_path data/ \
--data_train train.txt\
--data_test test.txt\
--data_dev dev.txt\
--output_dir model \
--model_name_or_path michiyasunaga/BioLinkBERT-large \
--layers -1\
--subtoken_pooling first_last\
--hidden_size 256\
--learning_rate 5e-5\
--use_crf False
```
