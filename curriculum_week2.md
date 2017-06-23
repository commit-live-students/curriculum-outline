# Week 2: Introduction to Machine Learning

* [Day 1] Feature Selection
* [Day 2] The Machine Learning Workflow (putting it all together with sklearn)
    - Complete the remaining parts of the ML Workflow (diagram)
         * Metrics
              - Overview and classification of metrics
              - Metrics for Regression
              - Metrics for Classification - binary
              - Metrics for Classification - multiclass
              - Metrics for other purposes (kappa etc)
         * Sampling
             - Basic Sampling methods (train-validation-test)
             - Advanced Sampling methods (Cross-Validation) - build intuition by reminding of statistical tests
             - Bootstrapping
         * Training Models
         * Hyperparameter Tuning
    - Putting it all together
         * A discussion on ML glossary from Linear Algebra perspective (and Linear Algebra basics)
         * Formulation of Machine Learning as an optimization problem
             - linear regression
             - support vector machines (hinge loss)
             - decision trees
             - Introduction to optimization algorithms
                 * GD
                 * Quadratic
    - A review of how it all fits in together by working through a dataset
         * The Complete Data Science/Machine Learning Workflow
              - Understanding the business context
                  * Demonstrate how the same ML task could be different depending on the business objective
                  * Have to think about deployment (model consumption) even before collecting data
                  * Choosing evaluation metric
              - Collecting Data
              - Exploratory Data Visualization
              - Data pre-processing
              - Feature Extraction
              - Sampling
              - Model Training and Tuning
              - Model Assessment
              - Model Deployment
              - Importance of having a Pipeline
    - [Hands-on]
         * Linear Algebra basics
         * Calculating Metrics for given data (structures)
         * Reproducing key plots used throughout the day
         * Industry Dataset Part 1 (EDA, FE)
* [Day 3] Machine Learning and sklearn (improving the workflow with sklearn expert features)
    - Understanding and adapting sklearn api
         * How to manage datasets with sklearn bunches
         * Creating synthetic datasets for experiments
         * Understanding the Estimator api for machine learning algorithms
         * Understanding Pipelines
             - Introduction to Pipelines
             - Pipelines and Feature Preprocessing
             - Pipelines and Feature Selection
             - Pipelines and Cross-Validation
             - Pipelines and Hyperparameter Tuning
             - Pipelines and Training Reports
             - Pipelines and Leakage
         * How to write your own estimator and use it with Pipeline and CrossValidation
    - Putting it all together with sklearn (end-to-end example on a dataset)
    - [Hands-on] Industry Dataset Portfolio Project
         * Portfolio Project: Using Pipelines to test multiple models on a single dataset
         * Create synthetic datasets that match given statistical properties from the industry dataset
         * Create plots to match given images of synthetic datasets
* [Day 4] Processing Image and Video Data
    - Walk-through: Create face detectors
         * Get started with OpenCV for image processing basics
             - IO
             - Datastructures
             - [Colorspaces]()
             - [Geometric Transformations](http://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_imgproc/py_geometric_transformations/py_geometric_transformations.html#geometric-transformations)
             - [Thresholding](http://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_imgproc/py_thresholding/py_thresholding.html#thresholding)
         * User Haar cascades to detect faces
         * Introduce image processing techniques to improve image quality for better face detection
         * Quick introduction to video-processing workflow (extract, transform, merge)
         * Do face detection/tracking on video
    - Image classification (MNIST) with Linear Regression! (flatten the image)
    - Introduction to alternatives
         * sk-image
         * TensorFlow and Keras
    - Some common transformations in image processing
    - Introduction to bag-of-visual-words (optional)
    - [Hands-on]
         * [Extend the face detection example to face and eye detection](http://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_objdetect/py_face_detection/py_face_detection.html)
         * Guided walk-through towards lane-detection
* [Day 5] Processing Text Data
    - Teaxt-to-features using sklearn api
    - Overview of a simple text extraction pipeline (tokenization, lemmatization etc)
    - Text extraction pipeline using NLTK
    - Text extraction pipeline using Spacy
    - Text extraction pipeline using TextBlob
    - Worked out Supervised ML problem on text data (reuters)
    - [Hands-on] Portfolio Project with Industry Dataset (Haptik)
         * Build a classifier for Haptik Dataset 
