**Name**: Handi Xie  
**Email**: hxie13@bu.edu  
**LinkedIn**: https://www.linkedin.com/in/handi-xie

This is my attempt to compete for BitGrit's Competition #18. I have used an employeed both classical machine learning methods, deep learning methods and ensemble methods for the competition, and utilized Google Colab's Pro+ for my development. If you ran into any trouble, please feel free to contact me by my email or linkedin.  

**Competition**: BitGrit's Competition #18
> Generative AI Competition: Detect the AI-generated photos  
> https://bitgrit.net/competition/18

**Requirments**

* Google Colab Pro
* Mount Google Drive to Google Colab 

**Instructions**

1. Please open http://colab.research.google.com.
2. Please drag and upload AGI\_Competition\_Handi\_Xie.ipynb via Upload.
3. Please upload the two folders ./models, ./Datasets to your Google Drive. For example, upload it to the Colab Notebook folder in your Google Drive.
4. Please save your Google Drive path to the global variable **gdrive_path**. For example, mine is 

> gdrive_path = '/content/drive/MyDrive/Colab Notebooks/Competition/CS523'

5. Then open Google Colab and follow the rest of instructions on the AGI\_Competition\_Handi\_Xie.ipynb as it contains both instructions on how the data pipeline works and the code for the data pipeline.

**Warning**

Pleaes don't run section 0x03 Model Training since training and tuning models take time and computational units. Instead, please load from /models.

**Architecture**

I have used the ensemble stacking model for my final submission.

For base estimators (level 0), I have used **PyCaret** to create a list of traditional machine learning models: CatBoost, LightGBM, Linear Regression, K Nearest Neighbours, Multiple Layered Perceptions, XGBoost. I have also used **TabNet**, a SOTA neural network model for tabular data developed by Google.

For meta estimator (level 1), I have used, Logistic Regression from scikit learn.

Please read

* AGI\_Competition\_Handi\_Xie\_print.pdf
* or
* AGI\_Competition\_Handi\_Xie.ipynb

for specific instructions