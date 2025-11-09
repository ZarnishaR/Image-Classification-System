# Cat vs. Dog Image Classification

This is a computer vision project to classify images as either cats or dogs, inspired by the [Kaggle Dogs vs. Cats competition](https://www.kaggle.com/c/dogs-vs-cats/overview/description).

## Quick Prediction

Run the prediction script:
```
python predict.py
# Example prompt:
Where is your image path?
samples/dog.jpg
# Output:
This image shows a dog
```

## Approach

- Built a Convolutional Neural Network (CNN) for image classification.
- Enhanced accuracy by applying VGG-16 (transfer learning) — a proven deep learning architecture ([VGG-16 paper](https://arxiv.org/abs/1409.1556)).
- For more details, see [Dog_vs_Cat.ipynb](https://github.com/patrick013/Image-Classification-CNN-and-VGG/blob/master/Dog_vs_Cat.ipynb).

**VGG-16 Architecture:**
![VGG](https://neurohive.io/wp-content/uploads/2018/11/vgg16-1-e1542731207177.png)

**Training Results (VGG16, 20 epochs):**
![result](https://raw.githubusercontent.com/patrick013/Image-Classification-CNN-and-VGG/master/pictures/a.png)

## Lessons Learned

A key challenge was stagnant loss during VGG training. The fix: ensure `y` labels are one-hot encoded!

## Reference

Simonyan & Zisserman, "Very Deep Convolutional Networks for Large-Scale Image Recognition." [arXiv:1409.1556](https://arxiv.org/abs/1409.1556)

---

_Adapted for Zarnisha_
