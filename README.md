# ObjectDetectionTests
Object Detection in realtime using some pretrained models like SSD, RFCN, FasterRFCN &amp; SSD_InceptionV2, trained with COCO

I use Anaconda Python and Tensorflow 1.5, as well as Nvidia GTX970. However since no training is needed, only classification calls, a CPU has to be enough. Remember to activate tensorflow environment on anaconda.

You have to download first the pretrained models. Here we use: 
http://download.tensorflow.org/models/object_detection/ssd_mobilenet_v1_coco_2017_11_17.tar.gz
http://download.tensorflow.org/models/object_detection/faster_rcnn_inception_resnet_v2_atrous_coco_2018_01_28.tar.gz
http://download.tensorflow.org/models/object_detection/ssd_inception_v2_coco_2017_11_17.tar.gz
http://download.tensorflow.org/models/object_detection/rfcn_resnet101_coco_2018_01_28.tar.gz
and unzip as follows:

SSD_GRAPH_FILE = 'ssd_mobilenet_v1_coco_2017_11_17\\frozen_inference_graph.pb'

RFCN_GRAPH_FILE = 'rfcn_resnet101_coco_2018_01_28\\frozen_inference_graph.pb'

FASTER_RCNN_GRAPH_FILE = 'faster_rcnn_inception_resnet_v2_atrous_coco_2018_01_28\\frozen_inference_graph.pb'

SSD_INCEPTION_GRAPH_FILE = 'ssd_inception_v2_coco_11_06_2017\\frozen_inference_graph.pb'


Then execute "jupyter notebook ObjectDetection.ipynb" from your console and play ! There are up to 10 images from the simulator located inside "images_finalP/*.png"

From my experience, I think the pretrained SSD_inception_V2 is fast (like SSDv1) and also detects small signals. SSDv1 fails on that, although it is not a big problem I guess.
I think no further training is needed for simulator. Don't know on real environment.
