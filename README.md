## Performance Comparison of Binary Classification Models

This project focuses on evaluating the performance of various convolutional neural network (CNN) architectures and configurations on a binary classification task. The models tested include variations of VGG, transfer learning approaches, and a custom MLP model. The study aims to analyze the impact of model depth, data augmentation, and transfer learning strategies on classification accuracy and efficiency.

Dataset Creation

The dataset was created based on the first names of the group members, selecting two classes of images representing the initials. For instance:
	•	Vulture vs. Rat for names starting with “V” and “R.”
	•	Vada Pav vs. Roti for other examples.

The dataset contains:
	•	100 images per class (200 total).
	•	Training set: 80 images per class.
	•	Testing set: 20 images per class.

Images were collected using:
	•	Bulk Image Downloader Script.
	•	DuckDuckGo Images Repository.

## Models and Configurations

The following models were trained and evaluated:
	1.	VGG (1 block)
	2.	VGG (3 blocks)
	3.	VGG (3 blocks) with data augmentation
	4.	Transfer learning with VGG16/VGG19 (all layers fine-tuned)
	5.	Transfer learning with VGG16/VGG19 (only final MLP layers fine-tuned)

A custom MLP model with comparable parameters to VGG16 was also developed for performance comparison.

Evaluation Metrics

Each model was evaluated on the following metrics:
	•	Training Time
	•	Training Loss
	•	Training Accuracy
	•	Testing Accuracy
	•	Number of Model Parameters

Results were tabulated for easy comparison.

Visualization with Tensorboard

Tensorboard was used for detailed performance tracking and visualization:
	1.	Scalars:
	•	Training loss vs. iterations.
	•	Training accuracy vs. iterations.
	•	Testing accuracy vs. iterations.
	2.	Images:
	•	Predictions on the test set visualized alongside actual labels.

Insights and Observations

The project investigates key insights such as:
	•	Impact of data augmentation: Does it improve model performance?
	•	Effect of fine-tuning duration: How does the number of epochs influence accuracy?
	•	Model confusion: Analysis of images where the model struggles to classify correctly.

Image Generation and Testing

To test model robustness:
	•	Images were generated with tools like DALL·E or similar.
	•	Prompts created:
	•	Class A: easy to classify.
	•	Class A: hard to classify.
	•	Class B: easy to classify.
	•	Class B: hard to classify.

Model performance on these sets of images was recorded and analyzed.

Conclusion

The study concludes with a comparison between the MLP model and VGG variants, analyzing factors like architecture complexity, transfer learning strategies, and augmentation benefits. Key findings and recommendations are presented based on experimental results.
