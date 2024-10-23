# Grad-CAM Analysis of ConvNeXt Models

## Overview

This repository contains the analysis and results of a Grad-CAM study performed on a subset of 70 patients, utilizing approximately 200 images. The analysis focuses on five ConvNeXt models trained on five specific labels. Grad-CAM was run on the images corresponding model of the  label.

## Dataset

- **Patients:** 70
- **Total Images:** ~200
- **Labels:** 5 (specific to the study)

## Methodology

The Grad-CAM (Gradient-weighted Class Activation Mapping) technique was used to visualize the areas of the input images that were significant for model predictions. The analysis was conducted on the rows where labels were present, using the corresponding ConvNeXt model associated with each label.

### Grad-CAM Implementation

1. **Model Selection:** For each labeled image, the specific ConvNeXt model trained on that label was used.
2. **Grad-CAM Execution:** Grad-CAM was applied to generate heatmaps that indicate which parts of the image contributed most to the model's predictions.

## Color Scale

The color scale used in the Grad-CAM visualizations ranges from low to high activation, represented by the following color gradient:

- **Low Activation:** Blue
- **Medium Activation:** Yellow
- **High Activation:** Red

This gradient allows for easy interpretation of which areas of the image are being emphasized by the model.

## Example Results

Here are links to specific Grad-CAM images generated during the analysis:

### AP
- ![Grad-CAM Image for AP/12339843](AP/12339843_x/ad08ee6f-3c1b04b7-2fffc4c7-03dba6ac-0a0fe4c7/grad_cam_AP_j_CNN_Label_1_convnext_base_ad08ee6f-3c1b04b7-2fffc4c7-03dba6ac-0a0fe4c7.jpg)
- ![Grad-CAM Image for AP/13909489](AP/13909489_x/1e26a41e-4119379e-ea086f9e-7fc0dac6-19175661/grad_cam_AP_j_CNN_Label_1_convnext_base_1e26a41e-4119379e-ea086f9e-7fc0dac6-19175661.jpg)
- ![Grad-CAM Image for AP/19820806](AP/19820806_x/31b1404b-e58bebb6-85516814-ef45404c-27ef252e/grad_cam_AP_j_CNN_Label_1_convnext_base_31b1404b-e58bebb6-85516814-ef45404c-27ef252e.jpg)
### Lateral
- ![Grad-CAM Image for LATERAL/11812752](LATERAL/11812752_x/1c7685ad-d09de1fd-b7d623d4-d650cad2-484f51c4/grad_cam_LATERAL_j_CNN_Label_5_convnext_base_1c7685ad-d09de1fd-b7d623d4-d650cad2-484f51c4.jpg)
- ![Grad-CAM Image for LATERAL/14080545](LATERAL/14080545_x/6a8da0b6-55a1a722-5bcb4ec9-ffeadb1a-e6645049/grad_cam_LATERAL_j_CNN_Label_5_convnext_base_6a8da0b6-55a1a722-5bcb4ec9-ffeadb1a-e6645049.jpg)
- ![Grad-CAM Image for LATERAL/16384927](LATERAL/16384927_x/5614a330-3ba5f58e-7c7e7bcb-7130e189-3a81b0c1/grad_cam_LATERAL_j_CNN_Label_5_convnext_base_5614a330-3ba5f58e-7c7e7bcb-7130e189-3a81b0c1.jpg)
### LL
- ![Grad-CAM Image for LL/12026649](LL/12026649_x/993c51b6-3bcd1ac8-5c1165ab-64dbc83f-0a808f66/grad_cam_LL_j_CNN_Label_1_convnext_base_993c51b6-3bcd1ac8-5c1165ab-64dbc83f-0a808f66.jpg)
- ![Grad-CAM Image for LL/15656471](LL/15656471_x/a7a942a4-e875dc07-a2b22a7b-2f399efe-a5564c6b/grad_cam_LL_j_CNN_Label_5_convnext_base_a7a942a4-e875dc07-a2b22a7b-2f399efe-a5564c6b.jpg)
- ![Grad-CAM Image for LL/10865278](LL/10865278_x/cbca7626-7f9ecc33-3dba643b-c5240b06-62f7c24e/grad_cam_LL_j_CNN_Label_1_convnext_base_cbca7626-7f9ecc33-3dba643b-c5240b06-62f7c24e.jpg)
### PA
- ![Grad-CAM Image for PA/11812752](PA/11812752_x/c87d8997-495ee626-930e6596-1f8d0a08-62fe7415/grad_cam_PA_j_CNN_Label_5_convnext_base_c87d8997-495ee626-930e6596-1f8d0a08-62fe7415.jpg)
- ![Grad-CAM Image for PA/12041908](PA/12041908_x/b5b965dc-9f27632c-954a7b1a-db0dc580-8285cae7/grad_cam_PA_j_CNN_Label_5_convnext_base_b5b965dc-9f27632c-954a7b1a-db0dc580-8285cae7.jpg)
- ![Grad-CAM Image for PA/17548402](PA/17548402_x/604a3890-13e97bde-c78246ae-d06e2f9c-1d737cee/grad_cam_PA_j_CNN_Label_5_convnext_base_604a3890-13e97bde-c78246ae-d06e2f9c-1d737cee.jpg)

## Conclusion

The analysis revealed that the ConvNeXt models tend to emphasize the borders of the images significantly. This tendency suggests that the models may be relying on specific viewpoints as shortcuts for prediction.


