 Adaptive Self-Learning Cobot Welding for Custom Fabrication

Intelligent Weld Quality Prediction and Adaptive Parameter Optimization

This project presents an explainable Machine Learning framework for adaptive robotic/cobot welding in custom fabrication environments.

The system is designed to predict whether a weld will **PASS or FAIL**, identify the primary reason for a predicted failure, recommend corrective welding parameters, optimize productivity, and learn from future production results.



 Problem Statement

Custom fabrication environments experience frequent variations in:

- Joint gap
- Material thickness
- Welding current
- Voltage
- Travel speed
- Wire feed rate
- Torch angle
- Weld distortion
- Component geometry and fit-up

Conventional robotic welding systems generally operate using predefined welding parameters. When fabrication conditions change, manual parameter adjustment or robot reprogramming may be required.

The proposed system provides an intelligent decision-support framework that enables a cobot to:

1. Predict weld quality.
2. Identify the reason for a predicted failure.
3. Recommend corrective parameter changes.
4. Prioritize which parameters should be changed first.
5. Maintain weld quality while improving productivity.
6. Learn from previous welding operations.



 Dataset

The model was developed using a welding production dataset containing 50 jobs.

### Input Features

The primary prediction model uses seven features:

Feature  Unit 
Current  A 
Voltage  V 
Travel Speed  mm/min 
Wire Feed Rate  m/min 
Torch Angle  ° 
Gap Size  mm 
Thickness  mm 

### Target

The target variable is:

PASS
FAIL

The dataset contains:

 34 PASS jobs
 16 FAIL jobs

Additional variables such as distortion and bead width are available in the dataset and are used for analysis, but the primary prediction model uses the seven process/fabrication parameters above.

Machine Learning Methodology

The project follows the following pipeline:

text
Historical Welding Data
        ↓
Data Cleaning
        ↓
Exploratory Data Analysis
        ↓
Correlation Analysis
        ↓
Feature Selection
        ↓
Model Training
        ↓
Model Evaluation
        ↓
Final Decision Tree
        ↓
New Job Prediction
        ↓
Failure Explanation
        ↓
Parameter Recommendation
        ↓
Productivity Optimization
        ↓
Learning From Actual Result
