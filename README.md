# Forward-Data-Lab-WebFormer

## Purpose

This project is to implement and test how the WebFomer model in this paper (https://arxiv.org/abs/2202.00217) works. More importanly, we want to see how the model would contribute in our Academic Online project. 

## Dependencies

- PyThon 3.9+
- PyTorch v2.0+
- lxml
- numpy
- spaCy
- sklearn

## Usage

For now, only the input layer can be run and tested. Type the command below to run the input layer code.

``` 
python "../Preprocess/[filename]" 
```

## File List
- Preprocess (the input layer)
  - html_tokenizer.py
  - main.py
  - parser.py
  - preprocess.py (tokenize and convert HTML and text to dimentional embeddings)
- Models
  - residual.py (feedforward layer)
  - transformer.py (stacked WebFormer layers)
  - rich_attn.py (attention layers)
- utils
  - tensor_utils.py (helper functions used in Models)

## Limitations and Improvements

Although the input layer is finished and can be run, the WebFormer layers are still being built. First off, we still need to test the attention and feedforward layers are working correctly. Also, since I referred to some TensorFlow code, we still need to refactor some codes from TensorFlow to PyTorch. Moreover, the output layer has not been implemented, and we still need to figure out how to import training data to train our model.
