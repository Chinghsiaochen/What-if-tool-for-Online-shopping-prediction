# Expanding AI Explainability and Model Transparency to All with Google What-If

*This project repository is created in partial fulfillment of the requirements for the Big Data Analytics course offered by the Master of Science in Business Analytics program at the Carlson School of Management, University of Minnesota*
![data_cloud_ai_summit max-2500x2500](https://github.com/Chinghsiaochen/What-if-tool-for-Online-shopping-prediction/assets/104823654/7522a095-5c26-4172-8bb6-86026c6758cd)

### Introduction: 
One challenge in Machine Learning is understanding of black-box classification and regression ML models. While these models demonstrate high accuracy, however, lack of transparency making it difficult for stakeholders to interpret and trust their outcomes in their decision-making processes. One powerful solution for addressing this challenge is Google What-If Tool. This tool serves as a resource for testing ML model performance in different scenarios, assessing the significance of different data features, and visualizing data across various models.

The primary goal of Google What-If Tool is to empower individuals, even those who without coding expertise, to explore trained ML models through a user-friendly interface. As for technical experts, Google What-If can integrate with TensorBoard and use with your model deployed on cloud AI platform.

![1_asnFlkSAHTD-Vde41sM5lg](https://github.com/Chinghsiaochen/What-if-tool-for-Online-shopping-prediction/assets/104823654/c5a7e8c9-596a-46b3-961b-640da8e08cb3)

### Set up instruction: 
1. Set-up: Install the required witwidget package
2. Loading data: Prepare dataset in a TFRecord file which can be accessed by the TensorBoard web server
3. Model Configuration: Configure for your particular scenario on how the tool will interact with your models and set up invoking methods for WitConfigBuilder object 
4. TensorFlow Serving: Have a ML model served on TensorFlow Serving using the classify, regress, or predict API
5. Cloud AI Platform Prediction: Utilize models deployed on Cloud AI Platform Prediction by employing the set_ai_platform_model method
6. Custom Prediction Functions: Define your own custom prediction function. In our demo, for example, we integrate SHAP value with the What-If to build a customized function for explaining output of models by quantifying the feature importances
7. Displaying the Tool: Pass the WitConfigBuilder object to the WitWidget constructor

Another use case for Google What-if is to be utilized independently without a deployed model, allowing users to analyze datasets without the need for model deployment.

### Dataset
In our demonstration, we use Online Shoppers Purchasing Intention Dataset from UC Irvine Machine Learning Repository.
https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset

### Project Video
<img width="1221" alt="Screenshot 2023-12-06 at 5 13 53 PM" src="https://github.com/Chinghsiaochen/What-if-tool-for-Online-shopping-prediction/assets/104823654/f3066f10-3aa4-4158-a15c-950220e950ee">
https://www.youtube.com/watch?v=sIoayXDUe1Y

### Relevant resources:
- Official Website: https://cloud.google.com/blog/products/ai-machine-learning/introducing-the-what-if-tool-for-cloud-ai-platform-models
- Introduction for beginner: https://www.youtube.com/watch?v=qTUUwfG1vSs 
- Other reference: https://medium.com/@furcifer/explaining-trees-with-fasttreeshap-and-what-if-tool-dc0afde9613
  https://medium.com/p/6ec140d45967
