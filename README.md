# medical-image-segmentation-a-survey
medical image segmentation: a survey
medical image segmentation

Three architectures achieve good performance:

### encoder-decoder network

structure: input-conv-deconv-segmentation

Implementation: ultrasound-nerve-segmentation

<u-net Convolutional networks for biomedical image segmentation> propose skip-connect from encoder to decoder.

<V-net Fully Convolutional Neural networks for volumetric medical image segmentation>1. propose dice-coeff loss which is specially designed for medical image segmentation. 2. illustrate the idea of 3D convolution on a images volume.

Other useful paper:

<learning to refine object segments> have a similar skip-connect structure

<bayesian segnet>, symmetric upsampling. not as powerful as u-net.

<DHSnet: Deep Hierarchical Saliency Network for Saliency Object Detection> similar to medical image (predict single probability map)

### forward network

structure: input-conv-upsampling-refinement

Implementation: medical-image-segmentation

<Deeplab: Semantic Image Segmentation with Deep Convolutional Nets, Atrous Convolution, and Fully Connected CRFs> achieves best performance on PASCAL VOC segmentation challenge

<Shallow and Deep Convolutional Networks for Saliency Prediction> similar to medical image (predict single probability map)

<DCAN: Deep Contour-Aware Networks for Accurate Gland Segmentation> learning to predict coutour map and segmentation map.

<Learning to Segment Object Candidates>

### multitask network cascades

SDS first propose the task: <Simultaneous Detection and Segmentation>

Implementation: rpn_drn_new

<Instance-aware Semantic Segmentation via Multi-task Network Cascades> defeat segmentation-only encoder-decoder network on COCO segmentation challenge

Miscellaneous

Dilated convolution helps reduce computation
