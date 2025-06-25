

  <h1>🚀 Machine Learning Project Documentation</h1>

  <p>This project showcases two beginner-friendly machine learning tasks built with Python and scikit-learn:</p>
  <ul>
    <li><strong>Iris Flower Classification</strong> - Predict flower species using Decision Tree Classifier</li>
    <li><strong>Diabetes Progression Prediction</strong> - Predict disease progression using Linear Regression</li>
  </ul>

  <div class="section">
    <h2>📦 Technologies Used</h2>
    <ul>
      <li><strong>Language:</strong> Python 3.x</li>
      <li><strong>Libraries:</strong> scikit-learn, numpy, pandas</li>
      <li><strong>Environment:</strong> Works in Jupyter Notebook, VSCode, or standard Python scripts</li>
    </ul>
  </div>

  <div class="section">
    <h2>🌸 Iris Flower Classification</h2>
    <p>This task predicts flower species based on sepal and petal measurements.</p>
    <h3>Code Example:</h3>
    <pre><code>from sklearn.datasets import load_iris
from sklearn.tree import DecisionTreeClassifier

iris = load_iris()
model = DecisionTreeClassifier()
model.fit(iris.data, iris.target)

new_flower = [[5.1, 3.5, 1.4, 0.2]]
prediction = model.predict(new_flower)
print("Predicted Species:", iris.target_names[prediction[0]])</code></pre>

    <h3>Steps:</h3>
    <ul>
      <li>Load Iris dataset</li>
      <li>Train a Decision Tree Classifier</li>
      <li>Predict species for new flower measurements</li>
    </ul>
  </div>

  <div class="section">
    <h2>💉 Diabetes Progression Prediction</h2>
    <p>Predicts numeric disease progression based on 10 standardized medical features.</p>
    <h3>Code Example:</h3>
    <pre><code>from sklearn.datasets import load_diabetes
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split

# Load dataset
diabetes = load_diabetes()
X_train, X_test, y_train, y_test = train_test_split(diabetes.data, diabetes.target, test_size=0.2, random_state=42)

# Train model
model = LinearRegression()
model.fit(X_train, y_train)

# Predict for new patient (standardized features)
new_patient = [[0.05, -0.02, 0.06, 0.04, 0.03, -0.01, 0.02, 0.01, 0.03, -0.02]]
prediction = model.predict(new_patient)
print(f"Predicted Disease Progression: {prediction[0]:.2f}")</code></pre>

    <h3>Steps:</h3>
    <ul>
      <li>Load the Diabetes dataset</li>
      <li>Train Linear Regression model</li>
      <li>Provide new patient data (standardized features)</li>
      <li>Predict disease progression score</li>
    </ul>
  </div>

  <div class="section">
    <h2>⚙️ Setup & Installation</h2>
    <ol>
      <li>Ensure Python 3.x is installed</li>
      <li>Install required libraries:<br>
      <pre><code>pip install scikit-learn numpy pandas</code></pre></li>
      <li>Run the examples in a Python script or Jupyter Notebook</li>
    </ol>
  </div>

  <div class="section">
    <h2>💡 Notes</h2>
    <ul>
      <li>Iris Classification is a <strong>classification problem</strong></li>
      <li>Diabetes Prediction is a <strong>regression problem</strong></li>
      <li>Inputs for Diabetes must match standardized feature format</li>
      <li>This project is beginner-friendly and focuses on ML fundamentals</li>
    </ul>
  </div>

  <div class="section">
    <h2>📫 Contact</h2>
    <p>Have questions? Reach out or feel free to experiment with the code for deeper learning.</p>
  </div>

</body>
</html>
