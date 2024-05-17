# Hospital Length of Stay: A Predictive Tool


![myimage](https://bestpractice.bmj.com/info/wp-content/uploads/2020/08/iStock-1194838627-scaled.jpg)


## :hospital: Project Overview 

The goal of this project was to create a tool by developing a **supervised classification machine learning model** that can predict the hospital length of stay for patients who are scheduled for General Surgery Procedures. 

**Hospital bed shortages** have been a significant challenge in healthcare worldwide, exacerbated further by the impact of the Covid19 pandemic. Surgical procedures often face cancellations due to a lack of available beds to accommodate post-operative patients.

In this context, accurately predicting the length of stay for patients becomes crucial for hospitals and healthcare facilities. A reliable predictive tool can assist hospital administrators, bed managers and healthcare staff in managing bed capacity effectively. By having a better estimate of the length of stay, hospitals can optimize their bed and staff allocation, improve patient safety, and enhance overall financial and medical efficiency.


## :file_folder: Dataset 	

**VitalDB** (Vital Signs DataBase) is an open Dataset from Seoul National University Hospital, Seoul, Republic of Korea containing perioperative clinical information, laboratory results and intraoperative monitoring parameters of 6,388 surgical patients (general, thoracic, urologic, and gynaecologic) who underwent routine or emergency surgery. 

The dataset includes 73 columns with Clinical parameters, 196 intraoperative monitoring parameters and 34 columns with Laboratory results parameters. For this project only data for General Surgical Patients was selected and used.

[Dataset](https://vitaldb.net/dataset/?query=overview) available here.

[CSV Files](https://www.kaggle.com/datasets/kamyababedi/vitaldb?select=clinical_parameters.csv) available here.


### :lock: Conclusion 


- The **Random Forest Classifier** Model having an overall accuracy of **74%**, shows promise as a reliable tool that could be used by hospital administrators, bed managers and healthcare professionals for predicting different Hospital Lengths of Stay (Short, Medium or Prolonged) in surgical patients. By performing accurate predictions, it can contribute to a more effective management of hospital resources (human and material) and reduce costs.

- Model's true effectiveness can only be determined by assessing its performance on **real-world unseen patient data**. Given that the model was trained on data where synthetic samples were generated for the minority classes (using SMOTE) to address the class imbalance issue, particular attention should be given to its performance on the "Medium" and "Prolonged" Length of Stay classes.

- The model's predictions could also be utilized by patients preoperatively to inform them about whether their hospital stay will be short, medium, or prolonged through an **web application**, based on specific input parameters. Empowering patients with this information can help them be proactive in preparing for surgery, planning their recovery and reducing anxiety level.

- Also, patients with a higher likelihood of a **prolonged hospital stay** can be targeted by hospital staff in order to develop and implement strategies earlier to optimize their discharge planning, recovery and potentially continuing care after discharge at home through **telemedicine**. This approach not only optimizes patient care but also helps to free up hospital beds and prevents surgery cancellations that happens often due to lack of beds.
