# Custom Object Detection

### If you want to detect a custom object navigate to [CustomOD](https://github.com/hackobi/polyp-detection-tool/tree/master/CustomOD) and follow the `README.md` instructions
```
https://github.com/hackobi/polyp-detection-tool
```

### Step 1: Prepare custom object images
- Save photos of the custom object(s) that the model will detect in `jpg` or `png` format to `./data/raw` directory. The more complex an object is the more images are needed for successful detection.
- If your photos are big, consider resizing them to a smaller and uniformed size as this will improve training times. Save the photos to resize in `/data/raw` and run `resize_images.py` defining the output size and format i.e.
```
python resize_images.py --raw-dir ./data/raw --save-dir ./data/images --ext jpg --target-size "(800, 600)"
```
Alternatively save your custom object images in  `./data/images/` making sure to save around 80% - 90% of the images in `./data/images/train` and 10% - 20% in `./data/images/test`

### Step 2: Annotate images
- [labelImg](https://tzutalin.github.io/labelImg/) is a great tool to annotate images and automatically generate `xml` files which you'll need to save in the respective folders `./data/images/train` and `./data/images/test` folders.


- Once the train and test images with their respective annotations in xml format are saved in their respective folders `./data/images/train` and `./data/images/test` you'll have to commit and push them into your repository as Colab will fork your repository into the notebook.


### Step 3: Open [Colab Notebook](https://colab.research.google.com/github/hackobi/polyp-detection-tool/blob/master/tensorflow_object_detection_training_colab.ipynb).
- Make sure your to replace repository's url in the first section of the notebook
- Run all the cells
