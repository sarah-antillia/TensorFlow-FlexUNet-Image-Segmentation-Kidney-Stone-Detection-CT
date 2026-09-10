<h2>TensorFlow-FlexUNet-Image-Segmentation-Kidney-Stone-Detection-CT (2026/09/11)</h2>
Sarah T. Arai<br>
Software Laboratory antillia.com<br><br>
This is the first experiment of Image Segmentation for <b>Kidney Stone Detection CT</b> 
based on our <a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Model">
TensorFlowFlexUNet Image Segmentation Model</a> 
(TensorFlow Flexible UNet Image Segmentation Model for Multiclass), 
and a 512x512 pixels cropped PNG 
<a href="https://drive.google.com/file/d/19UaFOh-2N9TFecFJtDklDZhm57EejDwy/view?usp=sharing">
<b>Kidney-Stone-Detection-ImageMask-Dataset.zip</b></a> 
(<a href="https://creativecommons.org/licenses/by/4.0/">CC BY 4.0</a>)
, which was derived by us from <br><br>
<b>Stone</b> subset of 
<a href="https://www.kaggle.com/datasets/orvile/axial-ct-imaging-dataset-kidney-stone-detection/data">
<b>Axial CT Imaging Dataset (Kidney Stone Detection)
</b></a> by Orvile.<br><br>
<b>Actual Image Segmentation for Kidney-Stone-Detection Images of 512x512 pixels </b><br>
As shown below, the inferred masks predicted by our segmentation model trained on the dataset 
appear similar to the ground truth masks.
<br><br>
<table >
<tr>
<th width="320" height="20">Input: image</th>
<th width="320" height="20">Mask (ground_truth)</th>
<th width="320" height="20">Prediction:inferred_mask</th>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/images/1005.png" width="320" height="320"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/masks/1005.png" width="320" height="320"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test_output/1005.png" width="320" height="320"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/images/1964.png" width="320" height="320"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/masks/1964.png" width="320" height="320"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test_output/1964.png" width="320" height="320"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/images/2125.png" width="320" height="320"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/masks/2125.png" width="320" height="320"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test_output/2125.png" width="320" height="320"></td>
</tr>
</table>
<hr>
<br>
<h3>1  Dataset Citation</h3>
The dataset used here was derived from <br><br>
<b>Stone</b> subset of 
<a href="https://www.kaggle.com/datasets/orvile/axial-ct-imaging-dataset-kidney-stone-detection/data">
<b>Axial CT Imaging Dataset (Kidney Stone Detection)
</b></a> by Orvile.
<br><br>
The following explanation (excerpt) was taken from the website above.<br><br>
<b>About Dataset</b><br>
<b>Axial CT Imaging Dataset for AI-Powered Kidney Stone Detection</b><br>
<b>A Comprehensive CT Dataset for Deep Learning Research</b><br>
<br>
This dataset provides a high-quality collection of Axial CT scan images for kidney stone detection, carefully 
curated and labeled by experienced medical professionals. It consists of two main groups:
<br>
✅ Kidney Stone Present<br>
✅ No Kidney Stone<br>
<br>
<b>Description</b><br>
This dataset introduces a comprehensive CT scan image dataset focused on kidney stone detection, 
consisting of two groups: one from individuals diagnosed with kidney stones and the other from those 
without the condition. The dataset has been meticulously curated, verified, and labeled by experienced 
medical professionals, ensuring its high quality and reliability for both research and educational applications.<br>
 Collected from medical centers in Sulaimani and Rania, Kurdistan Region, Iraq, the dataset provides unique insights
  into the prevalence and characteristics of kidney stones in this region. <br>
  With 3,364 original CT images and 35,457 augmented images, it offers a valuable resource for developing 
  and evaluating deep learning algorithms for kidney stone detection. <br>
  The augmented images further increase their applicability for algorithm training, medical research, and 
  educational purposes. This dataset can potentially advance diagnostic tool development, 
enhance medical research, and serve as an educational resource for students studying kidney stones.
<br><br>

<b>License</b><br>
<a href="https://creativecommons.org/licenses/by/4.0/">Attribution 4.0 International (CC BY 4.0) </a>
</a> (Free to use for research and commercial applications with proper attribution)
<br>
<br>
<b> Citation</b><br>
Abdalla, Peshraw Ahmed; Mahmood, Bander Sidiq; Hama, Nawzad Rasul (2025), <br>
“Axial CT Imaging Dataset for AI-Powered Kidney Stone Detection: A Resource for Deep Learning Research”, <br>
Mendeley Data, V2, doi: 10.17632/fwhytt5mzd.2<br>
<br>
<h3>
2 Kidney-Stone-Detection ImageMask Dataset
</h3>
<h3>
2.1 Download ImageMask Dataset
</h3>
 If you would like to train this Kidney-Stone-Detection Segmentation model,
please down load our dataset <a href="https://drive.google.com/file/d/19UaFOh-2N9TFecFJtDklDZhm57EejDwy/view?usp=sharing">
<b>Kidney-Stone-Detection-ImageMask-Dataset.zip</b> 
</a>(<a href="https://creativecommons.org/licenses/by/4.0/">CC BY 4.0</a>) 
 on Google Drive,
expand the downloaded, and put it under <b>./dataset/</b> to be:
<pre>
./dataset
└─Kidney-Stone-Detection
    ├─test
    │   ├─images
    │   └─masks
    ├─train
    │   ├─images
    │   └─masks
    └─valid
        ├─images
        └─masks
</pre>
<br>
<b>Kidney-Stone-Detection Statistics</b><br>
<img src ="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/Kidney-Stone-Detection_Statistics.png" width="512" height="auto"><br>
<br>
As shown above, the number of images in the training and validation datasets is not large to use as a training set for our segmentation model.
<br><br>
<h3>
2.2 Derivation of Kidney-Stone-Detection ImageMask Dataset
</h3>
The folder structure of the <b>Kindy Stone Dataset</b> is as follows, but it contains no annotation(mask) files,
because it is an image classification dataset.<br>
<pre>
./Kindy Stone Dataset
    ├─Augmented Dataset
    │   ├─Non-Stone
    │   └─Stone
    │     
    └─Original Dataset
        │   ├─0.jpg
...
        │   └─nnnn.jpg
        │
        └─Stone
             ├─0.jpg
...
             └─1576.jpg
</pre>
<b>Step 1</b><br>
We generated a 512x512 pixels cropped PNG images from the JPG files in the <b>Original Dataset/Stone</b> folder.
<br><br>
<b>Step 2</b><br>
We generated the pseudo masks corresponding to the PNG images
by applying an inference (segmentation) method of
a pretrained model <a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-KSSD2025-Kidney-Stone-CT">
TensorFlow-FlexUNet-Image-Segmentation-KSSD2025-Kidney-Stone-CT
</a> to the PNG master, without human annotation experts.<br>
<br>
<b>Step 3</b><br>
We generated our own Kidney-Stone-Detection-ImageMask-Dataset from pairs of the cropped PNG images and 
the corresponding pseudo masks. However, we excluded all empty black masks and the corresponding images.
<br><br>
<h3>
2.3 Train Sample Images and Masks
</h3>

<b>Train sample images</b><br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/asset/train_images_sample.png" width="1024" height="auto">
<br>
<b>Train sample masks</b><br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/asset/train_masks_sample.png" width="1024" height="auto">
<br>
<h3>
3 Train TensorFlowFlexUNet Model
</h3>
 We trained the Kidney-Stone-Detection TensorFlowFlexUNet model using the 
<a href="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/train_eval_infer.config"> <b>train_eval_infer.config</b></a> file. <br>
Please move to ./projects/TensorFlowFlexUNet/Kidney-Stone-Detection and run the following bat file.<br>
<pre>
>1.train.bat
</pre>
This simply runs the following command.<br>
<pre>
>python ../../../src/TensorFlowFlexUNetTrainer.py ./train_eval_infer.config
</pre>
<hr>

<b>Model parameters</b><br>
Defined a small <b>base_filters=16</b> and a large <b>base_kernels=(9,9)</b> for the first Conv Layer of Encoder Block of 
<a href="./src/TensorFlowFlexUNet.py">TensorFlowFlexUNet.py</a> 
and a large <b>num_layers=8</b> (including a bridge between Encoder and Decoder Blocks).
<pre>
[model]
image_width    = 512
image_height   = 512
image_channels = 3
input_normalize = True
normalization  = False
num_classes    = 2
base_filters   = 16
base_kernels  = (9,9)
num_layers    = 8
dropout_rate   = 0.03
dilation       = (1,1)
</pre>
<b>Learning rate</b><br>
Defined a small learning rate.  
<pre>
[model]
learning_rate  = 0.0001
</pre>
<b>Loss and metrics functions</b><br>
Specified "categorical_crossentropy" and "dice_coef_multiclass".<br>
<pre>
[model]
loss           = "categorical_crossentropy"
metrics        = ["dice_coef_multiclass"]
</pre>
<b >Learning rate reducer callback</b><br>
Enabled the learning_rate_reducer callback and a small reducer_patience.
<pre> 
[train]
learning_rate_reducer = True
reducer_factor     = 0.4
reducer_patience   = 4
</pre>
<b>Early stopping callback</b><br>
Enabled early stopping callback with patience=10 parameter.
<pre>
[train]
patience      = 10
</pre>
<b>Infer section</b><br>
<pre>
[infer] 
images_dir    = "./mini_test/images/"
output_dir    = "./mini_test_output/"
</pre>
<b>RGB color map</b><br>
RGB color map dict for Kidney-Stone-Detection 1+1 classes.<br>
<pre>
[mask]
mask_file_format = ".png"
;Kidney-Stone-Detection 1+1
rgb_map {(0, 0, 0): 0, (255, 255, 255):1}
</pre>
<b>Epoch change inference callbacks</b><br>
Enabled epoch_change_infer callback.<br>
<pre>
[train]
epoch_change_infer     = True
epoch_change_infer_dir =  "./epoch_change_infer"
epoch_change_infer     = False
epoch_change_infer_dir =  "./epoch_change_infer"
num_infer_images =  6
</pre>
By using this <b>epoch_change_infer</b> callback, on every epoch_change, the <b>infer</b> method of the 
<a href="./src/TensorFlowFlexModel.py">TensorFlowFlexModel</a> class 
can be called
 for 6 images in <b>mini_test</b> folder specified in <b>tiledinfer</b> section. This will help you confirm how the predicted mask changes 
 at each epoch during your training process.<br> <br> 
<b>Epoch_change_inference output at starting (1,2,3)</b><br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/asset/epoch_change_infer_at_start.png" width="1024" height="auto"><br>
<br>
<b>Epoch_change_inference output at ending (15,16,17)</b><br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/asset/epoch_change_infer_at_middlepoint.png" width="1024" height="auto"><br>
<br>
<b>Epoch_change_inference output at ending (32,33,34)</b><br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/asset/epoch_change_infer_at_end.png" width="1024" height="auto"><br>

<br>
In this experiment, the training process was stopped at epoch 34 by EarlyStoppingCallback.<br><br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/asset/train_console_output_at_epoch34.png" width="1024" height="auto"><br>
<br>
<a href="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/eval/train_metrics.csv">train_metrics.csv</a><br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/eval/train_metrics.png" width="520" height="auto"><br>

<br>
<a href="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/eval/train_losses.csv">train_losses.csv</a><br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/eval/train_losses.png" width="520" height="auto"><br>
<br>
<h3>
4 Evaluation
</h3>
Please move to a <b>./projects/TensorFlowFlexUNet/Kidney-Stone-Detection</b> folder, 
and run the following bat file to evaluate the TensorFlowFlexUNet model for Kidney-Stone-Detection.<br>
<pre>
>./2.evaluate.bat
</pre>
This bat file simply runs the following command.
<pre>
>python ../../../src/TensorFlowFlexUNetEvaluator.py  ./train_eval_infer.config
</pre>
Evaluation console output:<br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/asset/evaluate_console_output_at_epoch34.png" width="1024" height="auto">
<br><br>Image-Segmentation-Kidney-Stone-Detection

<a href="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/evaluation.csv">evaluation.csv</a><br>
The loss (categorical_crossentropy) to the tiledly split <b>Kidney-Stone-Detection/test</b> was very low, and dice_coef_multiclass 
very high, as shown below.
<br>
<pre>
categorical_crossentropy,0.0007
dice_coef_multiclass,0.9997
</pre>
<!--
<b>Why was the loss so low and the dice_coef so high in the evaluation scores for the test dataset in this segmentation model? </b><br>
The main reason is that the number of black pixels in the Background class is overwhelmingly larger than that of 
white pixels in the Stone class in almost all annotation (mask) data. 
As a result, the Background would be better recognized than the Stone in this multiclass FlexUNet model.
<br>
-->
<br>
<h3>5 Inference</h3>
Please move to a <b>./projects/TensorFlowFlexUNet/Kidney-Stone-Detection</b> folder, and run the following bat file to infer segmentation regions for images using the trained TensorFlowFlexUNet model for Kidney-Stone-Detection.<br>
<pre>
>./3.infer.bat
</pre>
This simply runs the following command.
<pre>
>python ../../../src/TensorFlowFlexUNetInferencer.py ./train_eval_infer.config
</pre>
<hr>
<b>mini_test_images</b><br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/asset/mini_test_images.png" width="1024" height="auto"><br>
<b>mini_test_mask(ground_truth)</b><br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/asset/mini_test_masks.png" width="1024" height="auto"><br>
<hr>
<b>Inferred test masks</b><br>
<img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/asset/mini_test_output.png" width="1024" height="auto"><br>
<br>
<hr>
<b>Enlarged images and masks for Kidney-Stone-Detection of 512x512 pixels</b><br>
As shown below, the inferred masks predicted by our segmentation model trained on the dataset appear similar to the ground truth masks.
<br>
<br>
<table>
<tr>
<th>Input: image</th>
<th>Mask (ground_truth)</th>
<th>Prediction: inferred_mask</th>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/images/1017.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/masks/1017.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test_output/1017.png" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/images/1311.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/masks/1311.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test_output/1311.png" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/images/1684.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/masks/1684.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test_output/1684.png" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/images/1800.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/masks/1800.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test_output/1800.png" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/images/1964.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/masks/1964.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test_output/1964.png" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/images/2411.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test/masks/2411.png" width="320" height="auto"></td>
<td><img src="./projects/TensorFlowFlexUNet/Kidney-Stone-Detection/mini_test_output/2411.png" width="320" height="auto"></td>
</tr>
</table>
<hr>
<br>
<h3>
References
</h3>
<b>1. KSSD2025: A New Annotated Dataset for Automatic Kidney Stone Segmentation and Evaluation With Modified U-Net-Based Deep Learning Models</b><br>
Murillo F. Murillobouzon; Paulo H. S. de Santana; Gabriel N. Missima; Weverson S. Pereira; Fernando P. Rivera; Gilson A. Giraldi<br>
<a href="https://ieeexplore.ieee.org/document/11165055">https://ieeexplore.ieee.org/document/11165055</a>
<br><br>
<b>2. A deep learning system for automated kidney stone detection and volumetric segmentation on noncontrast CT scans</b><br>
Daniel C. Elton, Evrim B.Turkbey, Perry J.Pickhardt, Ronald M.Summers<br>
<a href="https://www.moreisdifferent.com/assets/my_papers/B_AI_medical_imaging/2022_Z_Elton_Medical_Physics_kidney_stone_detector.pdf">
https://www.moreisdifferent.com/assets/my_papers/B_AI_medical_imaging/2022_Z_Elton_Medical_Physics_kidney_stone_detector.pdf</a>
<br><br>
<b>3. TensorFlow-FlexUNet-Image-Segmentation-Mendeley-Kidney-Stone-CT</b><br>
Toshiyuki Arai <br>
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Mendeley-Kidney-Stone-CT">
https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Mendeley-Kidney-Stone-CT
</a>
<br><br>
<b>4. TensorFlow-FlexUNet-Image-Segmentation-KSSD2025-Kidney-Stone-CT</b><br>
Toshiyuki Arai <br>
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-KSSD2025-Kidney-Stone-CT">
https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-KSSD2025-Kidney-Stone-CT
</a>
<br>
<br>
<b>5. TensorFlow-FlexUNet-Image-Segmentation-Kidney-Stone-CT-Axial</b><br>
Toshiyuki Arai <br>
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Kidney-Stone-CT-Axial">
https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Kidney-Stone-CT-Axial</a>
<br><br>
<b>6. TensorFlow-FlexUNet-Image-Segmentation-Model</b><br>
Toshiyuki Arai <br>
<a href="https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Model">
https://github.com/sarah-antillia/TensorFlow-FlexUNet-Image-Segmentation-Model
</a>
<br>
<br>
