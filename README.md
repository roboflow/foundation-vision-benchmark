# foundation-vision-benchmark

A qualitative set of tests for use in evaluating the capabilities of foundation vision models.

## 📝 Abstract

In 2023, multimodal vision models have become substantially more powerful; the year has been coined as the "year of multimodality." Roboflow actively explores new vision models and their capabilities, conducting qualitative tests to learn more about how different models perform.

Our tests help us answer questions like "will this model help with labeling data?" and "could this model be used in a two-stage detection system (i.e. OCR)?"

This repository contains several tests we have run on foundation vision models to understand their performance. If you are curious about exploring new vision models, this repository may give you direction, ideas, and result in novel learnings about the model with which you are working.

## ✅ Tests

| Task Type | Prompt        | Image               |
|-----------|---------------|---------------------|
| Classification   | What is in the image? Return the class of the object in the image. Here are the classes: Tesla Model 3, Toyota Camry. You can only return one class from that list. | ![Image Example](https://lh7-us.googleusercontent.com/-sp5y_4HnZrQeqbC4Ufb-CnHDBkG1uZT5E-A6LDEItuFzk4rxkoC-RFyL7xuzGKJZ029Zwbcyvip-dHrFX8lCbW7da1MRK97bORbaVrZdiUzRFhoSM-bwp3TgoNJKUxQHuMcC9fJpHAyLnaO1ig_MlQ)  |
| Classification   | What is in the image? Return the class of the object in the image. Here are the classes: pizza, deep dish pizza. You can only return one class from that list. | ![Image Example](https://lh7-us.googleusercontent.com/dxD4vgo4fMWSF32Uxh6eB8Bjj85Gfrm9lgSgCuH0KWJYhv4khZ9SfC9OMpOB0ResXi8npF5gEL3A0GZC9sqq-V-NlM19WBn1GIop59IdPqUbO29FhUvCbVZJZkZmjsAWM6BCEbTCNoK22hezBSD_sKo)  |
| Optical Character Recognition (Documents)   | Read the text in the image. | ![Image Example](https://media.roboflow.com/swift.png)  |
| Object Detection | Detect a dog on the image. Provide me with x_min_y_min, x_max and y_max coordinates. | ![Image Example](https://media.roboflow.com/dog.jpeg) |

## 🧪 Test Surface Area

We test:

1. Object detection
2. Classification
4. Document OCR
5. Handwriting OCR
6. Math OCR

See the sections below for reference images and prompts.

### General Recommendations

We also recommend testing visual question answering (asking general questions about an image), exploring areas such as:

- Spatial awareness: Can the model answer questions about how objects relate?
- Veracity: When asked a question about an image, is the model correct?
- Comprehensiveness: Does a model provide a comprehensive answer to your question? Are details missed?
- Consistently: Does a model consistently answer questions it can answer? Does a model say it cannot help with a question with which it has previously helped?

## ⚠️ Limitations

Given the vast array of possibilities with vision models, no set of tests, this one included, can comprehensively evaluate what a model can do; this repository is a starting point for exploration.

## 🦸 Contribute

We would love your help in making this repository even better! Whether you want to
add a new experiment or have any suggestions for improvement,
feel free to open an [issue](https://github.com/roboflow/awesome-openai-vision-api-experiments/issues)
or [pull request](https://github.com/roboflow/awesome-openai-vision-api-experiments/pulls).
