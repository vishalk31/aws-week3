# Image Classification using AWS SageMaker

The following tasks are performed.
- A pretrained Resnet50 model from pytorch vision library is used in the project (
- Fine-tune the model with hyperparameter tuning and Network Re-shaping
- Implement Profiling and Debugging with hooks
- Deploy the model and perform inference

## Project Set Up and Installation
Enter AWS through the gateway in the course and open SageMaker Studio.
Download the starter files.
Download/Make the dataset available.

## Dataset
Udacity's Dog Classification Data set is used to complete the task.

The dataset used - > (https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).

### Dependencies

```
Pytorch AWS Instance
```
## Files Used in the notebook

- `hpo.py` 
- `train_model.py` 
- `endpoint_inference.py`
- `train_and_deploy.ipynb` 

## Hyperparameter Tuning
- The ResNet model represents the deep Residual Learning Framework to ease the training process.
- A pair of fully connected Neural Networks has been added on top of the pretrained model to perform the classification task with 133 output nodes.
- AdamW from torch.optm is used as an optimizer.

Is there some anomalous behaviour in your debugging output? If so, what is the error and how will you fix it?
- There is no smooth output line and there are different highs and lows for the batch sets.
  If not, suppose there was an error. What would that error look like and how would you have fixed it?
- A proper mix of the batches with shuffling could help the model learn better
- Trying out different neural network architecture.

  

