# Electro-AI
<p>
Electro AI is a deep learning model leveraging Recurrent Neural Networks (RNN) and Long Short-Term Memory (LSTM) networks to predict electricity consumption in Delhi. By incorporating key factors such as temperature, humidity, population growth, and real estate trends, the model delivers precise hourly, weekly, and yearly forecasts. Ideal for utility management, Electro AI optimizes power distribution, reduces outages, and enhances planning for energy providers. This model is designed to meet the challenges of dynamic urban environments, improving the efficiency and reliability of electricity supply.</p>
<h1>Dataset</h1>
<p>There is Four Types of Dataset Available Right now</p>
<ol>
    <li>AEP_hourly Energy Consumption Dataset from (2004-2018)</li>
    <li>Delhi Power Consumption Dataset based on Multiple factors(2014-2024) </li>
    <li>Dom_hourly Dataset  Energy Consumption Dataset from (2004-2018)</li>
    <li>PJME_hourly Dataset Energy Consumption Dataset from (2004-2018)</li>
</ol>
<h1>Training And Testing</h1>
    <h3>PJME_Hourly</h3>
    <h4>Energy Consumption Graph</h4>
        <img src = "/Images/energyconsumption graph.png" alt="DOM Energy Consumption Graph">
    <h4>Training</h4>
    <p>For the training of the Model We have taken data before 13-02-2017</p>
    <img src = "/Images/pjmetrainingandtesting.png" alt="DOM Energy Consumption Graph">
    <h4>Testing</h4>
    <p>For the testing of the Model We have taken Data after 13-02-2017</p>
    <img src = "/Images/pjmetrainingandtesting.png" alt="DOM Energy Consumption Graph">
    <p>As you can see partition line on the graph on the right side the orange region it is the Testing region.</p>
    <h3>DOM_Hourly</h3>
    <h4>Energy Consumption Graph</h4>
     <img src = "/Images/domenergy.png" alt="PJME Energy Consumption Graph">
    <h4>Training</h4>
    <p>For the training of the Model We have taken data before 13-02-2017</p>
    <img src = "/Images/trainingandtesting.png" alt="DOM Energy Consumption Graph">
    <p>As you can see partition line on the graph on the left side the blue region it is the training region.</p>
    <h4>Testing</h4>
    <p>For the testing of the Model We have taken Data after 13-02-2017</p>
    <img src = "/Images/trainingandtesting.png" alt="DOM Energy Consumption Graph">
     <p>As you can see partition line on the graph on the right side the orange region it is the Testing region<./p>
<h1>Models</h1>
<ol>
    <li><h3>RNN(Recurrent neural network)</h3></li>
    <p>A Recurrent Neural Network (RNN) is a type of neural network designed for sequential data, where connections form cycles, allowing it to retain information from previous inputs.</p>
    <ol>
        <li><h4>Layers</h4></li>
        <p>In our RNN model, we determined that using 7 layers provided the optimal balance for achieving high accuracy on both the DOM and PJME datasets. After experimenting with various configurations, we found that this specific architecture delivered the best performance, effectively capturing the necessary patterns in both datasets for accurate predictions. This approach allowed us to fine-tune the model to achieve robust results.</p>
       <li> <h4>Epoches</h4></li>
       <p>In our RNN model, we tested various epoch counts, including 15, 20, and 30, to identify the ideal number for training. After careful evaluation, we found that 32 epochs provided the optimal balance for effective learning, ensuring the model was sufficiently trained without overfitting, and achieving the best performance on both the DOM and PJME datasets.</p>
       <li><h4>Problem</h4></li>
       <p>RNNs struggle with learning long-term dependencies due to the vanishing gradient problem, where gradients become too small during backpropagation, making it difficult to update weights for earlier inputs in long sequences. LSTM networks address this by introducing memory cells with gates (input, forget, and output) that regulate the flow of information. This allows LSTMs to retain relevant information over longer time periods, effectively solving the issue of learning from long sequences.</p>
    </ol>
    <li><h3>LSTM(Long short-term memory)</h3></li>
    <p>Long Short-Term Memory (LSTM) is a specialized RNN variant that addresses the problem of long-term dependency by using memory cells to maintain information over longer sequences efficiently.</p>
    <ol>
        <li><h4>Layers</h4></li>
        <p>In our LSTM model, we determined that using 7 layers provided the optimal balance for achieving high accuracy on both the DOM and PJME datasets. After experimenting with various configurations, we found that this specific architecture delivered the best performance, effectively capturing the necessary patterns in both datasets for accurate predictions. This approach allowed us to fine-tune the model to achieve robust results.</p>
        <li><h4>Epoches</h4></li>
          <p>In our LSTM model, we tested various epoch counts, including 15, 20, and 30, to identify the ideal number for training. After careful evaluation, we found that 32 epochs provided the optimal balance for effective learning, ensuring the model was sufficiently trained without overfitting, and achieving the best performance on both the DOM and PJME datasets.</p>
    </ol>
</ol>
<h1>Prediction And Accuracy</h1>
<h1>Electro-AI Model Explanation</h1>
<h1>Experience The Models</h1>
    <h3>Model Video</h3>
    <h3>Model Link 👇</h3>

```
https://electroai.streamlit.app/
```
