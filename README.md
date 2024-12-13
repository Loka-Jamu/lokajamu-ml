![image](https://github.com/user-attachments/assets/986d579d-f951-4d14-9b7e-db94fb6d1389)# LokaJamu Machine Learning Part

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

## Model
Ingredients detection models were evaluated using pre-trained model mobilenetv2_1.00_224

     ```py
     model = tf.keras.Sequential([
          based_model,  # MobileNet V2
          tf.keras.layers.Flatten(),
          tf.keras.layers.Dense(128, activation='relu'),
          tf.keras.layers.BatchNormalization(),
          tf.keras.layers.Dense(7, activation='softmax') ])
     ```

After training the model and adjusting its settings, it can now recognize ingredients with over 90% accuracy.<br />
<img src="[https://github.com/AnimaLink/Machine-Learning-app/assets/91884661/99b70b64-bcc6-4a6f-b87d-2172e3f1358b](https://github.com/user-attachments/assets/52f89fff-918a-4eb4-980f-8c619d4b819b)"  width="auto" height="auto">








