# Image-Classification-with-Neural-Networks
Machine learning and deep learning methodologies for the classification of leaf species using a dataset of 99 classes, 990 images, and 192 extracted features

Key Methodologies

    Dimensionality Reduction & Feature Selection: Utilized PCA, t-SNE, and UMAP to visualize feature separability. t-SNE proved most effective for clustering. Feature selection was tested using Random Forest Classifiers with filter and wrapper methods.

    Multilayer Perceptron (MLP): Implemented as a baseline model using the 192 engineered features. Post-hyperparameter tuning, the MLP achieved high consistency with an average test accuracy of approximately 95.8% and significantly reduced computational time.

    CNN & Transfer Learning: Compared a CNN built from scratch against a VGG16 pretrained model. While the from-scratch CNN struggled (avg. accuracy ~48%), Transfer Learning reached average validation accuracies of approximately 78%.

    Explainable AI (XAI): Employed LIME (Local Interpretable Model-agnostic Explanations) to interpret model decisions. XAI revealed that hyperparameter tuning significantly increased the MLP’s confidence and the CNN’s ability to recognize relevant leaf features.

Core Conclusions

    Feature Engineering vs. Deep Learning: The MLP model using engineered features outperformed the Transfer Learning models, demonstrating that well-defined features can dominate even complex pretrained models in small-dataset scenarios.

    Efficiency of Transfer Learning: Transfer Learning proved far more effective than training a CNN from scratch when training data is limited, improving accuracy by roughly 30%.

    Consistency through Tuning: Hyperparameter tuning for the MLP primarily improved result stability and consistency across trials rather than just peak accuracy.

Technologies Used

    Languages/Libraries: Python (Pandas, NumPy, Seaborn), Scikit-learn, TensorFlow/Keras.

    Models: MLP, CNN, VGG16, RandomForestClassifier.

    Tools: Google Colab, LIME

Contributors: Team of 5
