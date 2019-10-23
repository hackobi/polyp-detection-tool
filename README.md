# Polyp Detection Demo



## Usage

In a browser open and run the polyp detection tool [Colab Notebook](https://colab.research.google.com/github/hackobi/polyp-detection-tool/blob/master/tensorflow_object_detection_training_colab.ipynb).

### Requirements
The required packages will be installed in the Colab notebook





## Using a frozen TensorFlow graph to run inference locally

### Step 1: Download `frozen_inference_graph.pb`and ´label_map.pbtxt`

If you want to run inference on your local system you'll need the frozen inference graph and label map that you get after training. Feel free to try these which work well on polyp detection:

- [frozen_inference_graph.pb](https://github.com/hackobi/REPO/releases/)
- [label_map.pbtxt](https://github.com/hackobi/REPO/releases/)

### Step 2:


Run locally
```
local_inference_test.ipynb
```
