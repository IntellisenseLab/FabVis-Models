# Fabvis-Models

Clone the repository,

```sh
git clone https://github.com/IntellisenseLab/FabVis-Models.git
```

Download pretrained weight files from [here](https://drive.google.com/drive/folders/1JVNd73yBYyc2zmSpT_0xdXGlFTm3Aj2i?usp=sharing) or trained weight files from [here](https://drive.google.com/drive/folders/1T1TOtBPdqAKvcSKPr4Ck1FthdLoPeb5Y?usp=sharing) and extract them and move the each folder into the repo folder.


<br>

# Model Comparison

| Model            | Precision   | Recall      | F1-score    | mAP@0.5     |  Average IoU | Output |
| ---------------- | ----------- |------------ |------------ |------------ |------------   | ---------- |
| Yolov4-Tiny-Pretrained      |  0.35       |  0.1        | 0.15        | 0.1553      | 24.10        |   [chart](trainOutput/tiny-pretrained-chart.png)  [terminal](trainOutput/tiny-pretrained-terminal.png)     |
| Yolov4-Tiny-Not-Pretrained      |  0.35       |  0.1        | 0.15        | 0.1553      | 23.85        |   [chart](trainOutput/tiny-no-pretrained-chart.png)  [terminal](trainOutput/tiny-no-pretrained-terminal.png)     |

<br>

# Model Train Commands

Following commands will enable the training of models in coorindation of [Preprocess system](https://github.com/IntellisenseLab/FabVis-RD-Preprocess)

<br>

## Yolov4-Tiny

```sh
./darknet detector train ../config/obj.data ../Fabvis-Models/config/yolov4-tiny.cfg ../Fabvis-Models/preTrainedWeights/yolov4-tiny.conv.29 -dont_show -mjpeg_port 8090 -map
```

## Yolov4

```sh
./darknet detector train ../config/obj.data ../Fabvis-Models/config/yolov4.cfg ../Fabvis-Models/preTrainedWeights/yolov4.conv.137 -dont_show -mjpeg_port 8090 -map
```

## Yolov4x-mish

```sh
./darknet detector train ../config/obj.data ../Fabvis-Models/config/yolov4x-mish.cfg ../Fabvis-Models/preTrainedWeights/yolov4x-mish.conv.166 -dont_show -mjpeg_port 8090 -map
```

## Yolov4-csp-swish

```sh
./darknet detector train ../config/obj.data ../Fabvis-Models/config/yolov4-csp-swish.cfg ../Fabvis-Models/preTrainedWeights/yolov4-csp-swish.conv.164 -dont_show -mjpeg_port 8090 -map
```

## Yolov4-csp-x-swish

```sh
./darknet detector train ../config/obj.data ../Fabvis-Models/config/yolov4-csp-x-swish.cfg ../Fabvis-Models/preTrainedWeights/yolov4-csp-x-swish.conv.192 -dont_show -mjpeg_port 8090 -map
```

## Yolov4-csp

```sh
./darknet detector train ../config/obj.data ../Fabvis-Models/config/yolov4-csp.cfg ../Fabvis-Models/preTrainedWeights/yolov4-csp.conv.142 -dont_show -mjpeg_port 8090 -map
```

## Yolov4-p5

```sh
./darknet detector train ../config/obj.data ../Fabvis-Models/config/yolov4-p5.cfg ../Fabvis-Models/preTrainedWeights/yolov4-p5.conv.232 -dont_show -mjpeg_port 8090 -map
```

## Yolov4-p6

```sh
./darknet detector train ../config/obj.data ../Fabvis-Models/config/yolov4-tiny.cfg ../Fabvis-Models/preTrainedWeights/yolov4-p6.conv.289 -dont_show -mjpeg_port 8090 -map
```