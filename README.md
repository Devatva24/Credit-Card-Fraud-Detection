<h1>Credit Card Fraud Detection Using Machine Learning</h1>

<h2>📌 Objective</h2>
<p>Build a machine learning model capable of accurately detecting fraudulent credit card transactions to help financial institutions minimize fraud-related losses.</p>

<hr>

<h2>🛑 Problem Statement</h2>
<p>Credit card fraud is a major threat resulting in billions of dollars in losses each year.<br>
Fraudulent transactions are extremely rare compared to legitimate ones, making it a highly <b>imbalanced classification problem</b>.<br>
Traditional detection systems are insufficient — requiring a <b>machine learning</b> based, intelligent solution.</p>

<hr>

<h2>📊 Dataset</h2>
<ul>
  <li><b>Source</b>: <a href="https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud" target="_blank">Kaggle - Credit Card Fraud Detection Dataset</a></li>
  <li><b>Details</b>:
    <ul>
      <li>284,807 transactions recorded over two days.</li>
      <li>492 fraudulent transactions (only <b>0.172%</b> of all transactions).</li>
      <li>Features: Numerical values transformed via <b>PCA</b> (for confidentiality).</li>
      <li>Target:
        <ul>
          <li><code>Class = 0</code> → Legitimate</li>
          <li><code>Class = 1</code> → Fraudulent</li>
        </ul>
      </li>
    </ul>
  </li>
</ul>

<hr>

<h2>⚙️ Methodology</h2>

<h3>1. Data Preprocessing</h3>
<ul>
  <li>Load and explore the dataset.</li>
  <li>Handle class imbalance using <b>SMOTE</b>.</li>
  <li>Standardize/normalize features if necessary.</li>
  <li>Perform train-test split (with stratification).</li>
</ul>

<h3>2. Exploratory Data Analysis (EDA)</h3>
<ul>
  <li>Analyze class distribution.</li>
  <li>Study correlations and feature importance.</li>
  <li>Visualize transaction amount and transaction time.</li>
</ul>

<h3>3. Model Building</h3>
<ul>
  <li>Test multiple models:
    <ul>
      <li>Logistic Regression</li>
      <li>Decision Tree</li>
      <li>Random Forest</li>
      <li>XGBoost</li>
      <li>LightGBM</li>
      <li>Support Vector Machine (SVM)</li>
    </ul>
  </li>
  <li>Use cross-validation for evaluation.</li>
</ul>

<h3>4. Model Evaluation</h3>
<ul>
  <li>Use appropriate metrics for imbalanced data:
    <ul>
      <li>Precision</li>
      <li>Recall</li>
      <li>F1-Score</li>
      <li>ROC-AUC score</li>
      <li>Confusion Matrix</li>
    </ul>
  </li>
</ul>

<h3>5. Optimization</h3>
<ul>
  <li>Hyperparameter tuning (GridSearchCV/RandomizedSearchCV).</li>
  <li>Feature selection or engineering if needed.</li>
</ul>

<h3>6. Deployment (optional)</h3>
<ul>
  <li>Create a simple web app using Streamlit or Flask.</li>
  <li>Allow users to input transaction data and get a fraud prediction.</li>
</ul>

<hr>

<h2>🛠️ Technologies Used</h2>
<ul>
  <li>Python</li>
  <li>Libraries:
    <ul>
      <li>NumPy, Pandas</li>
      <li>Scikit-learn</li>
      <li>Matplotlib, Seaborn</li>
      <li>Imbalanced-learn (for SMOTE)</li>
      <li>XGBoost, LightGBM</li>
    </ul>
  </li>
  <li>Jupyter Notebook / Google Colab for experimentation</li>
  <li>(Optional) Streamlit or Flask for deployment</li>
</ul>

<hr>

<h2>🚧 Challenges</h2>
<ul>
  <li>Extremely imbalanced dataset.</li>
  <li>Need to minimize false negatives (missing frauds).</li>
  <li>Achieving high recall without too many false positives.</li>
</ul>

<hr>

<h2>✅ Results</h2>
<ul>
  <li>Best-performing model achieved:
    <ul>
      <li>High Recall (&gt; 90%) for fraud detection.</li>
      <li>Good Precision to reduce unnecessary alarms.</li>
      <li>ROC-AUC score above 0.95.</li>
    </ul>
  </li>
</ul>

<hr>

<h2>📝 Conclusion</h2>
<p>The project demonstrates that machine learning models can effectively detect fraudulent credit card transactions even in highly imbalanced datasets. 
With real-world deployment, such systems can significantly help banks and financial institutions reduce fraud losses.</p>

<hr>

<h2>🔮 Future Work</h2>
<ul>
  <li>Test on real-time streaming data.</li>
  <li>Combine models using ensemble techniques.</li>
  <li>Integrate anomaly detection algorithms.</li>
  <li>Deploy the model on a cloud platform for scalability.</li>
</ul>
