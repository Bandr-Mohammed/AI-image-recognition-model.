# AI-image-recognition-model

A keras AI image recognition model trained and tested to recognize and differentiate between Iphone and Samsung mobile phones.

## Steps for model creation and training

- Opening the TeachableMachin website
- Naming the classes (in this case "Iphone" and "Samsung") and uploading the images for its appropriate class.
- Then clicking the `Train Model` button in the "Training".

Like so:

![Image Alt](https://github.com/Bandr-Mohammed/AI-image-recognition-model./blob/main/Screenshot%20(5).png?raw=true)


- After training the model, we need to export the model by clicking the `Export Model` button.
- Then choosing the `Tensorflow` category and making sure the model conversion type is "keras".
- Finally, clicking on the `Download my model` button.

Like so:

![Image Alt](https://github.com/Bandr-Mohammed/AI-image-recognition-model./blob/main/Screenshot%20(6).png?raw=true)

## Steps for testing the model

- Copying the keras code from the TeachableMachin and pasting it into a GoogleColab notebook.

Like so:

![Image Alt](https://github.com/Bandr-Mohammed/AI-image-recognition-model./blob/main/Screenshot%20(7).png?raw=true)

- Upload an image for testing the model, as well as the extracted files from the downloaded "converted.keras" zip file.

Like so:

![Image Alt](https://github.com/Bandr-Mohammed/AI-image-recognition-model./blob/main/Screenshot%20(8).png?raw=true)

- Then applying the following changes to the code:

  - Add the line: `import tf_keras as tk`.
  - Change the line: `model = load_model("keras_Model.h5", compile=False)` to: `model = tk.models.load_model("keras_model.h5", compile=False)`.
  - Declare the path for the image used for testing (image should not have been used in training the model).

Like so:

![Image Alt](https://github.com/Bandr-Mohammed/AI-image-recognition-model./blob/main/Screenshot%20(9).png?raw=true)

## Test Result

![Image Alt](https://github.com/Bandr-Mohammed/AI-image-recognition-model./blob/main/Screenshot%20(10).png?raw=true)

The picture used for testing the model was an image of a Samsung phone, the model correctly classified and determined that the image belongs to the Samsung class.
