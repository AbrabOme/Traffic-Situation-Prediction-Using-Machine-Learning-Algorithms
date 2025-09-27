<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Traffic Situation Prediction Using Machine Learning</title>
</head>
<body style="font-family: Arial, sans-serif; line-height: 1.6; max-width: 900px; margin: auto;">

    <h1>Traffic Situation Prediction Using Machine Learning</h1>

    <p>
        This project implements and compares three machine learning algorithms — 
        <strong>K-Nearest Neighbors (KNN)</strong>, <strong>Decision Trees</strong>, and <strong>Random Forest</strong> — 
        to predict traffic situations based on vehicle counts and temporal features.
    </p>

    <h2>📌 Project Overview</h2>
    <p>
        Traffic prediction plays a key role in smart city planning, congestion reduction, and efficient 
        transportation management. In this project, we built a <strong>traffic situation classifier</strong> that 
        predicts one of four classes — <code>heavy</code>, <code>high</code>, <code>low</code>, or <code>normal</code> traffic — 
        using a dataset of 2,976 traffic records.
    </p>

    <p>Our pipeline includes:</p>
    <ul>
        <li><strong>Data Cleaning:</strong> Duplicate removal, missing value handling, and correction of inconsistent records</li>
        <li><strong>Outlier Detection &amp; Removal:</strong> Using the IQR method to improve data quality</li>
        <li><strong>Feature Engineering:</strong> Temporal feature extraction, quantile-based binning, total vehicle count feature</li>
        <li><strong>Class Imbalance Handling:</strong> SMOTE to generate synthetic samples for minority classes</li>
        <li><strong>Feature Scaling:</strong> Standardization for better model performance, particularly for KNN</li>
    </ul>

    <h2>🧠 Machine Learning Models</h2>
    <p>We implemented and compared three models:</p>
    <ul>
        <li><strong>KNN (k=5):</strong> Baseline model using majority vote of nearest neighbors</li>
        <li><strong>Decision Tree:</strong> Simple yet interpretable model with recursive feature-based splits</li>
        <li><strong>Random Forest (100 estimators):</strong> Ensemble approach for better accuracy and reduced overfitting</li>
    </ul>

    <h2>📊 Results</h2>
    <table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; text-align: center;">
        <thead>
            <tr>
                <th>Model</th>
                <th>Accuracy</th>
                <th>Weighted Precision</th>
                <th>Weighted Recall</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>KNN</td>
                <td>82.93%</td>
                <td>0.86</td>
                <td>0.83</td>
            </tr>
            <tr>
                <td>Decision Tree</td>
                <td>85.34%</td>
                <td>0.86</td>
                <td>0.85</td>
            </tr>
            <tr>
                <td><strong>Random Forest</strong></td>
                <td><strong>88.79%</strong></td>
                <td><strong>0.89</strong></td>
                <td><strong>0.89</strong></td>
            </tr>
        </tbody>
    </table>

    <p>
        Random Forest outperformed the other models, demonstrating the effectiveness of 
        ensemble learning for traffic prediction tasks.
    </p>

    <h2>🚀 Future Work</h2>
    <ul>
        <li>Hyperparameter tuning for further performance gains</li>
        <li>Integration of additional features (weather, events, road conditions)</li>
        <li>Experimenting with deep learning models (e.g., LSTMs)</li>
        <li>Building a real-time traffic prediction dashboard</li>
    </ul>

    <h2>👥 Contributions</h2>
    <p>This project was developed collaboratively by:</p>
    <ul>
        <li><strong>Tazower Rahman Sowad</strong></li>
        <li><strong>Kazi Abrab Hossain</strong></li>
        <li><strong>Md. Abrar Rahman Shafin</strong></li>
        <li><strong>Md. Fardin Hassan Tamim</strong></li>
    </ul>

</body>
</html>
