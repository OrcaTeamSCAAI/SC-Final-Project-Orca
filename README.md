# Binary Classification of Artificially Preserved Fruits vs Naturally Fresh Fruits

## Project Description
Projek ini bertujuan untuk menciptakan sebuah model AI yang dapat melakukan tugas binari klasifikasi dengan arsitektur CNN untuk mengklasifikasikan buah apel yang segar secara alami dengan buah apel yang terlihat segar dengan zat pengawet yang berlebihan.

## Contributor
| Full Name | Affiliation | Email | LinkedIn | Role |
| --- | --- | --- | --- | --- |
| Kevin Raihan Yassin| Startup Campus, AI Track | raihankevin14@gmail.com | [link](https://www.linkedin.com/in/kevraihany) | Team Lead |
| Larasati | Startup Campus, AI Track | yayaslarasati881@gmail.com | [link](https://www.linkedin.com/in/larasati-yayas-485ab0278?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app) | Team Member |
| Safina Octaviana Putri | Startup Campus, AI Track | safinaoctavianap@gmail.com | [link](https://www.linkedin.com/in/safinaoctav-4747r) |Team Member |
| Muhammad Roihan Fuady | Startup Campus, AI Track | muhammadroihanf99@gmail.com | [link](https://www.linkedin.com/in/mrfuadyy) | Team Member |
| Najla Qurrata Aini Putri Yusrizal | Startup Campus, AI Track | najlaqurrata@gmail.com | [link](https://www.linkedin.com/in/najla-qurrata-aini-putri-yusrizal-25571228b) | Team Member |
| M.Fadhlul Rahman Prabowo | Startup Campus, AI Track | fadhlulrahman687@gmail.com | [link](https://www.linkedin.com/in/fadhlul-rahman-a0787b262/) | Team Member |

## Setup
### Prerequisite Packages (Dependencies)
- pandas==2.1.0
- openai==0.28.0
- google-cloud-aiplatform==1.34.0
- google-cloud-bigquery==3.12.0
- ...
- ...

### Environment
| | |
| --- | --- |
| CPU | Example: Apple M3 Pro 12-core CPU |
| GPU | Example: Nvidia A100 (x1) |
| ROM | Example: 1 TB SSD |
| RAM | Example: 36 GB |
| OS | Example: macOS Sonoma v14.1.1 |

## Dataset
Describe your dataset information here. Provide a screenshot for some of your dataset samples (for example, if you're using CIFAR10 dataset, then show an image for each class).
- Dataset 1 Link: [https://...](https://app.roboflow.com/kevin-raihan-jklv5/fruit-yztjl/5)
  ![Pict Dataset 1](https://github.com/OrcaTeamSCAAI/SC-Final-Project-Orca/blob/main/Pict%20dataset%201.png)
- Dataset 2 Link: [https://...](https://app.roboflow.com/rahmans11-rn9us/apel-classify/2)
  ![Pict Dataset 2](https://github.com/OrcaTeamSCAAI/SC-Final-Project-Orca/blob/main/Pict%20dataset%202.png)

## Results
### Model Performance
Describe all results found in your final project experiments, including hyperparameters tuning and architecture modification performances. Put it into table format. Please show pictures (of model accuracy, loss, etc.) for more clarity.

#### 1. Metrics
Inform your model validation performances, as follows:
- For classification tasks, use **Precision and Recall**.
- For object detection tasks, use **Precision and Recall**. Additionaly, you may also use **Intersection over Union (IoU)**.
- For image retrieval tasks, use **Precision and Recall**.
- For optical character recognition (OCR) tasks, use **Word Error Rate (WER) and Character Error Rate (CER)**.
- For adversarial-based generative tasks, use **Peak Signal-to-Noise Ratio (PNSR)**. Additionally, for specific GAN tasks,
  - For single-image super resolution (SISR) tasks, use **Structural Similarity Index Measure (SSIM)**.
  - For conditional image-to-image translation tasks (e.g., Pix2Pix), use **Inception Score**.

Our Model Specify.

| model | epoch | learning_rate | batch_size | optimizer | val_loss | val_precision | val_recall | ... |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Densenet121 | 200 |  0.001 | 50 | Adam | --- | 83.50% | 66.50% | ... |
| LeNet | 200 | 0.001 | 50 | Adam | --- | 87.50% | 87.50% | ... |


#### 2. Ablation Study
Any improvements or modifications of your base model, should be summarized in this table. Feel free to adjust the columns in the table below.

| model | layer_A | layer_B | layer_C | ... | top1_acc | top5_acc |
| --- | --- | --- | --- | --- | --- | --- |
| vit_b_16 | Conv(3x3, 64) x2 | Conv(3x3, 512) x3 | Conv(1x1, 2048) x3 | ... | 77.43% | 80.08% |
| vit_b_16 | Conv(3x3, 32) x3 | Conv(3x3, 128) x3 | Conv(1x1, 1028) x2 | ... | 72.11% | 76.84% |
| ... | ... | ... | ... | ... | ... | ... |

#### 3. Training/Validation Curve
Insert an image regarding your training and evaluation performances (especially their losses). The aim is to assess whether your model is fit, overfit, or underfit.

Model DenseNet Eval

![Model LeNet Eval](https://github.com/OrcaTeamSCAAI/SC-Final-Project-Orca/blob/main/DenseNet%20Model%20Eval.png)

Model LeNet Eval

![Model LeNet Eval](https://github.com/OrcaTeamSCAAI/SC-Final-Project-Orca/blob/main/LeNet%20Model%20Eval.png)
 
### Testing
Show some implementations (demos) of this model. Show **at least 10 images** of how your model performs on the testing data.

Gambar dibawah ini adalah hasil percobaan kami terhadap model yang telah kami buat, kelas 0 merupakan predikisi untuk kelas ARTIFISIAL sedangkan kelas 1 untuk kelas NATURAL
![Model Test](https://github.com/OrcaTeamSCAAI/SC-Final-Project-Orca/blob/main/Testing%20Model.jpeg)

### Deployment (Optional)
Describe and show how you deploy this project (e.g., using Streamlit or Flask), if any.

Model yang telah kita buat untuk saat ini kami deploy menggunakan streamlit

Link Deployment Streamlit [https://colab.research.google.com/drive/1L7dmIjkVVvImdP-oZEbq3ozs69m5aS6I?hl=id]

## Supporting Documents
### Presentation Deck
- Link: [(https://drive.google.com/drive/u/2/folders/1ocDRb6U28rhvdmFnPtIlIv4WTLYglW7g)]

### Business Model Canvas
Provide a screenshot of your Business Model Canvas (BMC). Give some explanations, if necessary.
![Bussines Model Canvas](https://github.com/OrcaTeamSCAAI/SC-Final-Project-Orca/blob/main/BMC.png)

### Short Video
Provide a link to your short video, that should includes the project background and how it works.
- Link: [https://...](https://www.youtube.com/watch?v=r4BY5qf_xVg)

## References
Provide all links that support this final project, i.e., papers, GitHub repositories, websites, etc.
- Link: https://...
- Link: https://...
- Link: https://...

## Additional Comments
Provide your team's additional comments or final remarks for this project. For example,
1. Model DenseNet : Link: [https://colab.research.google.com/drive/1kysPGZkrsLYz6n7IhZMgCJZHUIoqaRKs?hl=id]
2. Model LeNet : Link: [https://colab.research.google.com/drive/1kuVexzMlRVgJcTkB6CIkPv8fGZLS36J6?hl=id#scrollTo=UI1Ksn7eB8Zy]
3. Model Deployment in Streamlit : Link:[https://colab.research.google.com/drive/1L7dmIjkVVvImdP-oZEbq3ozs69m5aS6I?hl=id]

## How to Cite
If you find this project useful, we'd grateful if you cite this repository:
```
@article{
...
}
```

## License
For academic and non-commercial use only.

## Acknowledgement
This project entitled "Binary Classification of Artificially Preserved Fruits vs Naturally Fresh Fruits" is supported and funded by Startup Campus Indonesia and Indonesian Ministry of Education and Culture through the "**Kampus Merdeka: Magang dan Studi Independen Bersertifikasi (MSIB)**" program.
