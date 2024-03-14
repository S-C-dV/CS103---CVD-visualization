# Cardiovascular disease risk factors visualisation given smoker status

## Description

<p>This project analyses the data provided by the "Cardiovascular disease dataset" provided on <a href="https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset">kaggle</a>.</p>
<p> From the csv file, we read and parsed the data into a Patient data type comprised of relevant tuple subclasses. From this list of new patient data, we filtered the impossible values. For example, we removed patients with height measurements that are greater than the world record. However, any values that weren't impossible were kept in the data set regardless of the unlikelihood of their occurence as we did not have any evidence to point to valid mistakes in data collection.</p>
<p>The main purpose of this project is to create a bar chart demonstrating the proportions of patients for each risk factor within their smoker status, separated by age ranges that the user selects.</p>
<p>This project uses course-specific modules, and thus may not be able to import the proper packages. I aim to rebuild this project to be more publicly accessible in the future. Additionally, I hope to increase the efficiency of the code as I see opportunity for such improvements as my knowledge increases.</p>
<h2>Demonstration</h2>
<p>This project is run using the main(file,age) function. The function reads the file provided and filters the data for the age range that contains the age given by the user. The age ranges are:
<ul>
    <li>18-35</li>
    <li>36-50</li>
    <li>51-65</li>
    <li>66-80</li>
    <li>81+</li>
</ul>
</p>
<p>For example, here is the bar chart produced when searching the data set for age 40.</p>
<img src="./images/CS103 CVD 40yrs.png"/>
<p><br/>Additionally, as age 45 is in the same range, the output will be the same:</p>
<img src="./images/CS103 CVD age45.png"/>
<p><br/>In contrast, the proportions are different when observing a different age range, such as 18-35 when inputting age 25:</p>
<img src="./images/CS103 CVD age25.png"/>
<p></br>Here, as there were no reasonable patients in this age range with CVD, the bars are removed. This is another area of improvement to explicitly differenciate between 0% proportions and a simple lack of patients to begin with.</p>