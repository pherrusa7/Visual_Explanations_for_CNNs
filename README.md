# Visual_Explanations_for_CNNs
I did research in all kind of visual explanations for CNNs since saliency maps and another techniques ending up with Grad-CAM, the newer, which I have implemented a general version that can be used for any model in keras.

Here you can find a presentations with a summary of a the seven I believe more powerful methods to this end (**visual_explanations_via_gradient.pdf**), and the implementation of a general grad-CAM from the implementation of @jacobgil in https://github.com/jacobgil/keras-grad-cam/blob/master/grad-cam.py (**grad_cam.py**)

Execution:
python grad_cam.py new_boat.jpg

If you want to use your own model, only import the file and use the following call:

general_gradCAM(model, preprocessed_input, predicted_class, model_generator, weights=None, original_im=None,
                     block_CAM="block5_conv3", nb_classes = 1000, size=224)
