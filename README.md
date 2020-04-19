# Skin Lesion Classification using CNN


Skin cancer represents a major public health concern as it affects many people in Canada and around the world, where it is the most common of all cancer types. If a patient with a pigmented lesion could be identified as someone with or at a risk of developing skin cancer, then measures could be taken right away to lower their risk or destroy the cancer if developed at an early stage. Thus, a reliable and automatic skin lesion classification system would be essential in detecting a malignancy. In this project, Convolutional Neural Networks (CNN) were utilized to accurately classify pigmented skin lesions in dermoscopic images to detect the malignant skin lesions as early as possible. CNNs excels in analyzing visual imagery as they are fully connected feed forward neural networks that reduce the number of parameters very efficiently without losing out on the quality of models. 

The data set used in this project is “The HAM10000 dataset, a large collection of multi-source dermoscopic images of common pigmented skin lesions”, which can be found under the `data` folder.
[P. Tschandl, C. Rosendahl and H. Kittler, "The HAM10000 dataset, a large collection of multi-source dermatoscopic images of common pigmented skin lesions", Scientific Data, vol. 5, no. 1, 2018. Available: 10.1038/sdata.2018.161.](https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000)

The HAM10000 dataset was first pre-processed via data editing and cleaning, then split into the feature and target values, before applying feature normalization and data augmentation. A basic CNN architecture was built to be employed against the processed data set images to classify their respective skin lesion category, alongside InceptionV3, ResNet152V2, and VGG16, which were pre-trained CNN models on the ImageNet data set. Hyperparameters were pre-selected and kept constant across all models. Weights were added to address the major class imbalance in the data set, by making the models more sensitive to Melanocytic nevi [nv] as it represented around two-thirds of the data. Evaluation results showed that the basic CNN's performance was comparable to InceptionV3 and ResNet152V2, and closely competing with our tweaked VGG16 model which topped all our scoring metrics, scoring weighted 88.54\% accuracy, 87.76\% precision, 88.74\% recall, and 87.69\% f1-score. However, according to the confusion matrices and classification accuracy plots, it could be seen that the more training data available for the skin lesion category, the better the models were at predicting them during test time. More malignant skin lesion images had to be provided for more accurate results and better malignancy classification, as the main aim in the medical field is to reduce the number of patients dying. Overall, this project demonstrated CNN's potential in the context of disease classification to lead further advances in the medical field with its image recognition abilities.

You can find the written IEEE format journal paper for this project `Skin_Lesion_Classification_using_Convolutional_Neural_Networks.pdf` under the main directory. The paper is organized as follows: <br />
• Section I: Introduction <br />
• Section II: Background & Evaluation Metrics <br />
• Section III: Related Work <br />
• Section IV: Data Set <br />
• Section V: Data Pre-Processing <br />
• Section VI: Models and Implementations <br />
• Section VII: Results <br />
• Section VIII: Conclusions <br />
• Section IX: Future Work <br />

You can find the whole code for this project `Skin Cancer MNIST HAM10000-vFinal.ipynb` under the `Code` folder.





