# Model-Deployment-on-GCP-using-Streamlit-for-Resume-Parsing
Perform model deployment on GCP for resume parsing model using Streamlit App.

ARCHITECTURE DIAGRAM
![image](https://github.com/prerakchintalwar/Model-Deployment-on-GCP-using-Streamlit-for-Resume-Parsing/assets/54786504/b4d11f78-8833-4eda-b96e-33812defd8d4)


**Project Description**

**Business Objective**

The resume parser application can take in millions of resumes parse the needed fields and categorize them. We use popular python libraries like Spacy and OCR text classifications. In this project, for ML model deployment, there are two initial assumptions, first that there is an ML model built and, second, there is an interface available for the model (Streamlit app)

We aim to create the ML model deployment project by using the google cloud platform (GCP). Here, GCP is used as a cloud provider. But first, we would suggest you go through the former project, Resume parsing with Machine learning - NLP with Python OCR and Spacy, before starting this project.

 

**Aim**

To deploy the machine learning model for the ‘Resume parsing with Machine learning - NLP with Python OCR and Spacy’ project on Google Cloud Platform (GCP)

 

**Tech stack**

Language - Python
Services - GCP, Docker
 

**Approach**
Three components for ML model deployment

* Source repository
* Cloud build
* Virtual Machine
 

**Steps:**

1. Cloud Source Repository
* Create a new repository or Connect to an external repository
* Clone the repository
2. Git commands
* Upload the necessary files to the repository in zip format
* Unzip the folder and move to the git folder
* Follow steps (git commands) in order to add the files to the cloud source repository
3. CLOUD BUILD TRIGGER
* In your GCP console, create a new cloud build trigger.
* Run the trigger
4. Create a docker file
* Go to Google Container Repository (GCR) (Deployed images are stored)
5. Virtual Machine creation
* Create a VM instance
6. Server deployment 1 (server-based deployment
* Connect to VM instance
* Follow the steps given in the ‘setup-new-vm.sh’ file
* Once the above steps are successfully completed, go to the particular URL (copy the external IP code and port)
* This will direct you to the resume parse page, where we can add any resume document and extract the details.
7. Server deployment 2 (docker deployment)
* Connect to VM
* Follow the steps given in the ‘install-docker.sh’ file
* Pull the docker image from the container and run it on the VM
* Once the above steps are successfully completed, go to the particular URL (copy the external IP code and port)
* This will direct you to the resume parse page, where we can add any resume document and extract the details.
