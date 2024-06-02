# Data-Mining-Project
Using machine learning and data mining tools in Python to perform exploratory data analysis on a large dataset using Jupyter Notebook.

This was a group project developed in between four members. The file named Paper.pdf documents this. The division of labor for all tasks 
was as follows:

    My work:

        - Writing, developing, and testing the entirety of the Jupyter Notebook using the Jupyter Notebook tool in Anaconda 
        Distribution.

        - Writing sections IV and V of the paper, titled "Implementation" and "Results" respectively.

    Not my work (Handled by other group members):

        - Writing sections I, II, III, VI, VII of the paper.

This project requires two files to run:

    DataMiningProject.ipynb - Interactive Python Notebook file that takes in a specific dataset file named "GamingStudy_data.csv"
    as input, and performs exploratory data analysis on the information inside.

    GamingStudy_data.csv - Large dataset containing over 10,000 records of individual gaming habits and mental health 
    outcomes. Dataset source: https://osf.io/vnbxk/ (Also documented in "DataMiningProject.ipynb").

To run the project:

    This project runs on Jupyter Notebook using the scikit-learn package. In order to run this, scikit-learn needs to be installed
    in your environment, and the third cell needs to be modified. The modifications that need to be made to the third cell are as 
    follows:

        The third cell contains the following line of code: 
        
            df = pd.read_csv(r'C:\Users\SampleUser\Downloads\GamingStudy_data.csv', encoding='unicode_escape')

        The raw string literal in first argument passed must be replaced with the absolute filepath of the GamingStudy_data.csv
        file on your own machine. For instance, for mine, it might like something like this after I download it:

            df = pd.read_csv(r'C:\Users\JonathanGuzman\Downloads\GamingStudy_data.csv', encoding='unicode_escape')

        Or like this if I place it within a dedicated folder somewhere:

            df = pd.read_csv(r'C:\Users\JonathanGuzman\Datasets\GamingStudy_data.csv', encoding='unicode_escape')

    Once scikit-learn is installed, the dataset is downloaded onto your device, and the read_csv() function call has been modified
    to include the absolute filepath on your device, the project can be run using the .ipynb IDE of your choice. This project was 
    developed using Jupyter Notebook on the Anaconda Distribution platform, and can be run there.
