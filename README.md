# tf2.x_expts
Getting used to Tensor Flow 2.x

I have been working on Chopin Nocturnes and the Rubber Band Gun and fell behind on Tensor Flow 2.x.

Still want to do the Cartoonify camera and have some new ideas to add. However, I need to get up to speed on Tensor Flow 2.x.
- https://github.com/Mark-MDO47/Cartoonify

For my own education and amusement I am starting with this Google Colab project:
- https://github.com/tensorflow/hub/blob/master/examples/colab/object_detection.ipynb

Because the original project used the "Apache License, Version 2.0" I am continuing that.
- You may obtain a copy of the License at
  - http://www.apache.org/licenses/LICENSE-2.0

For my own sanity I am keeping the original file object_detection.ipynb and working on my own version mdo_object_detection.ipynb. I will develop on Google Colab but plan to implement on the amazing Nvidia Jetson Nano (I still have the previous A02 hardware).
- https://www.nvidia.com/en-us/autonomous-machines/embedded-systems/jetson-nano/

In order to have a local copy of the Tensorflow Hub model(s) so I could run the camera without an internet connection:
- original URL in code was: https://tfhub.dev/google/openimages_v4/ssd/mobilenet_v2/1
- download from modified URL: https://tfhub.dev/google/openimages_v4/ssd/mobilenet_v2/1?tf-hub-format=compressed
- expand 1.tar.gz to disk area: D:\2020-04-26_TF_models\TensorFlowHub_models\inception_resnet_v2
- use this instead of original URL in code: D:/2020-04-26_TF_models/TensorFlowHub_models/inception_resnet_v2
- it looks like this:
  - $ ls -ltr "D:\2020-04-26_TF_models\TensorFlowHub_models\inception_resnet_v2"
  - total 280429
  - -rw-r--r-- 1 mdo 197609 287156985 Sep  7  2018 saved_model.pb
  - -rw-r--r-- 1 mdo 197609         2 Sep  7  2018 tfhub_module.pb
  - drwxr-xr-x 1 mdo 197609         0 May  3 21:37 assets/
  - drwxr-xr-x 1 mdo 197609         0 May  3 21:37 variables/

See this: https://stackoverflow.com/questions/50322001/how-to-save-load-a-tensorflow-hub-module-to-from-a-custom-path
