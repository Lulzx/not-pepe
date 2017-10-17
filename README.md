not-pepe
---

### Get your tensorflow installed

[follow one of the guides here](https://www.tensorflow.org/install/)

### Train it

```
python retrain.py \
 --bottleneck_dir=bottlenecks \
 --model_dir=inception \
 --summaries_dir=training_summaries/long \
 --output_graph=retrained_graph.pb \
 --output_labels=retrained_labels.txt \
 --image_dir=images
```

### Classify it

```
python label_image.py image.jpg
```

### Example output

```
(tensorflow) $ python label_image.py test-image.jpg
PEPE
(tensorflow) $ python label_image.py catte.png
NOT PEPE
```
