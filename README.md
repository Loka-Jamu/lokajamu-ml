# LokaJamu Machine Learning Part

## Team Member

|          Name         | Bangkit-ID |       Path       |
|:---------------------:|:----------:|:----------------:|
|  Alfian Diva Awangga  |  M587B4KY0356  | Machine Learning |
|  Wahyuni Fajrin Rosyidah  |  M587B4KX4461  | Machine Learning |
|   Diah Nur Astanti    |  M272B4KX1106  |  Machine Learning |

## Dataset
The dataset used for training, validating, and testing model consits 2590 images.
[Dataset Link](https://drive.google.com/drive/folders/1hnSqTgtMHFG2HYy9ayQctXj6X6dkaD4y?usp=drive_link)

|          Name         | Count | 
|:---------------------:|:----------:|
|  Asam Jawa  |  370  | 
|  Belimbing Sayur  |  370  | 
|   Jahe  |  370  | 
|  Jeruk Nipis  |  370  | 
|  Kunyit  |  370  | 
|   Lengkuas  |  370  | 
|   Serai  |  370  |

<img src="https://github.com/user-attachments/assets/f74715da-0ffb-448a-9a70-85a7aa6685b4"  width="350" height="350">

## Model
We used image classification with a transfer learning method, using MobileNetV2 as the base model. To improve its accuracy, we added extra layers and performed fine-tuning to adapt the model specifically to our jamu ingredient dataset. This helped the model recognize ingredients more precisely and effectively.

     ```
     model = tf.keras.Sequential([
          based_model,  # MobileNet V2
          tf.keras.layers.Flatten(),
          tf.keras.layers.Dense(128, activation='relu'),
          tf.keras.layers.BatchNormalization(),
          tf.keras.layers.Dense(7, activation='softmax') ])
     ```

After training the model and adjusting its settings, it can now recognize ingredients with over 90% accuracy.<br /> 
![image](https://github.com/user-attachments/assets/986d579d-f951-4d14-9b7e-db94fb6d1389)

### Model Performance
The performance of our model was evaluated using test data
![image](https://github.com/user-attachments/assets/8b5ff7a9-2b2b-4c4d-ab03-c131b629f7f0)
![image](https://github.com/user-attachments/assets/ad48c4f4-e59b-4512-ba38-56ec37185b1d)


## Requirements
To execute the notebook and use the model, the following dependencies are necessary:
- tensorflow
- numpy
- matplotlib
- seaborn
- scikit-learn
- ipywidgets
- ipython
- notebook

## Step to Classification
1. Clone the repository
```bash
git clone https://github.com/Loka-Jamu/lokajamu-ml.git
```
2. Install the required dependencies
```bash
pip install tensorflow numpy matplotlib seaborn scikit-learn ipywidgets ipython notebook
```
3. Open the notebooks
4. Set the dataset's source directory where it is stored
5. Execute the notebook cells to train the model and assess its performance

