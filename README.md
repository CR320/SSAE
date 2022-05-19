# SSAE
Existing methods of semi-supervised human pose estimation mainly focus on single-person pose estimation and only solve the task of keypoint detection. In multi-person scenes, these methods cannot be trained end-to-end and need to crop human instances out of the input image according to the annotated bounding boxes, which means raw unlabeled data cannot be directly exploited during training time. To leverage raw unlabeled data without any additional annotations, we propose an end-to-end trained semi-supervised method of multi-person human pose estimation for the first time. Our method is based on a one-stage paradigm that jointly performs keypoint detection and keypoint grouping. To leverage the unlabeled examples, our method conducts consistency regularization on heatmaps for keypoint detection and employs a pseudo-labeling approach based on keypoint clustering for keypoint grouping. We validate the effectiveness of our method on CrowdPose and COCO Keypoint benchmarks. Compared to the supervised baseline, our method significantly improves accuracy by +11.9 AP, +8.5 AP, and +6.2 AP on CrowdPose at 5\%, 10\% and 20\% labeling ratios, respectively. On the larger dataset COCO Keypoint, our method also effectively surpasses supervised baseline by +14.6 AP, +8.0 AP, and +6.0 AP at 1\%, 5\% and 10\% labeling ratios, respectively. Furthermore, compared to previous semi-supervised methods in a multi-stage paradigm, our method achieves higher AP gains at different labeling ratios and is more competitive in crowded scenes.
