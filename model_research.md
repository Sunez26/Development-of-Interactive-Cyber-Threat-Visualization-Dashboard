AI/ML Model Research
Development of Interactive Cyber Threat Visualization Dashboard
Introduction

This document explores various Machine Learning and Deep Learning models that can be applied to cyber threat detection and visualization. The models were evaluated based on their suitability for handling network traffic data, anomaly detection, scalability, and integration with an interactive dashboard system.

Model 1: Ridge Regression

Type: Supervised Learning
Used For: Regularized regression

Description:
Ridge Regression is an extension of linear regression that adds regularization to reduce overfitting by penalizing large coefficients.

Accuracy:
Improves stability compared to basic linear regression.

Advantages:

Reduces overfitting

Handles multicollinearity

Disadvantages:

Still limited to linear relationships

Applications:
Traffic trend prediction, resource usage forecasting

Model 2: AdaBoost

Type: Ensemble Learning
Used For: Classification

Description:
AdaBoost combines multiple weak classifiers to form a strong classifier by focusing more on previously misclassified data.

Accuracy:
High when properly tuned.

Advantages:

Improves weak learners

Good for structured datasets

Disadvantages:

Sensitive to noisy data

Applications:
Cyber attack classification

Model 3: Extra Trees (Extremely Randomized Trees)

Type: Ensemble Learning
Used For: Classification and regression

Description:
Extra Trees is similar to Random Forest but introduces more randomness when splitting nodes, which can improve generalization.

Accuracy:
High accuracy with reduced variance.

Advantages:

Faster than Random Forest

Less prone to overfitting

Disadvantages:

Slightly less interpretable

Applications:
Threat detection in network logs

Model 4: CatBoost

Type: Gradient Boosting
Used For: Classification

Description:
CatBoost is an advanced boosting algorithm optimized for handling categorical data efficiently.

Accuracy:
Very high predictive performance.

Advantages:

Handles categorical features automatically

Minimal preprocessing required

Disadvantages:

Requires computational resources

Applications:
Attack type classification

Model 5: LightGBM

Type: Gradient Boosting
Used For: Classification and regression

Description:
LightGBM is a fast gradient boosting framework that uses tree-based learning algorithms.

Accuracy:
High accuracy and fast training speed.

Advantages:

Efficient for large datasets

Low memory usage

Disadvantages:

Sensitive to parameter tuning

Applications:
Large-scale cyber threat prediction

Model 6: Isolation Forest

Type: Unsupervised Learning
Used For: Anomaly detection

Description:
Isolation Forest isolates anomalies instead of profiling normal data points, making it efficient for detecting unusual network behavior.

Accuracy:
Very effective for anomaly detection tasks.

Advantages:

Works well without labeled data

Fast execution

Disadvantages:

Does not classify attack types

Applications:
Network anomaly detection

Model 7: One-Class SVM

Type: Unsupervised Learning
Used For: Anomaly detection

Description:
One-Class SVM learns the boundary of normal data and identifies deviations as anomalies.

Accuracy:
Good for detecting rare attack patterns.

Advantages:

Suitable for fraud and intrusion detection

Disadvantages:

Computationally intensive

Applications:
Intrusion detection systems

Model 8: Convolutional Neural Network (CNN)

Type: Deep Learning
Used For: Pattern recognition

Description:
CNNs can detect spatial patterns in structured data and are sometimes adapted for cybersecurity feature maps.

Accuracy:
High with sufficient training data.

Advantages:

Captures complex feature interactions

Disadvantages:

Requires large dataset

High training cost

Applications:
Advanced threat pattern detection

Model 9: Gated Recurrent Unit (GRU)

Type: Deep Learning
Used For: Sequential data analysis

Description:
GRU is a simplified version of LSTM designed for time-series and sequential data processing.

Accuracy:
High for temporal cyber traffic patterns.

Advantages:

Faster than LSTM

Captures sequence dependencies

Disadvantages:

Complex implementation

Applications:
Real-time cyber attack monitoring

Model 10: Autoencoder

Type: Deep Learning
Used For: Unsupervised anomaly detection

Description:
Autoencoders learn compressed representations of normal data and detect anomalies based on reconstruction error.

Accuracy:
High anomaly detection performance.

Advantages:

Effective for unknown attack detection

Disadvantages:

Requires careful tuning

Applications:
Zero-day attack detection

Model Comparison

Supervised ensemble models such as LightGBM and CatBoost provide strong classification performance. Unsupervised models like Isolation Forest and Autoencoders are highly effective for detecting unknown threats. Deep learning models offer powerful pattern recognition but require significant computational resources.

Selected Model

Isolation Forest

Reason for Selection

Isolation Forest is selected because it efficiently detects anomalies without requiring fully labeled datasets. Since cyber attacks often involve unusual network behavior, anomaly detection plays a crucial role in identifying potential threats in real-time dashboard systems.

Application in the Project

In this project, the Isolation Forest model will analyze network traffic features to detect abnormal patterns. Detected anomalies will be visualized through the dashboard using interactive charts to support proactive monitoring and response.
