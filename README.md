# Graded Challenge 3

_Graded Challenge ini dibuat guna mengevaluasi pembelajaran pada Hacktiv8 Data Science Fulltime Program khususnya pada konsep Ensemble._

# Overall Analysis

#### Tentang Data
Dataset merupakan data untuk dapat memprediksi kelangsungan hidup pasien akibat gagal jantung. 

#### Sumber Data
Data asli berasal dari data kaggle dengan link: https://www.kaggle.com/andrewmvd/heart-failure-clinical-data

#### Objective
Membuat model klasifikasi untuk memprediksi kematian akibat Gagal Jantung.

#### Ukuran Data
Data memliki ukuran 299 rows dan 13 columns

#### Exploratory Data Analysis

Dari hasil visualisasi didapatkan informasi sebagai berikut:

* Jumlah pasien yang meninggal akibat gagal jantung adalah 96 pasien dan yang meninggal bukan akibat gagal jantung adalah 203 pasien
* Pasien dengan usia 55 tahun keatas memiliki kemungkinan meninggal akibat gagal jantung, sedangkan untuk pasien dengan usia 40 sampai 55 tahun memiliki kemungkinan kecil meninggal akibat gagal jantung
* Pasien yang menderita anaemie tidak memiliki pengaruh signifikan terhadap kematian akibat gagal jantung
* Pasien dengan tingkat enzim CPK dalam darah sampai dengan 1500 (mcg/L) memiliki kemungkinan resiko meninggal akibat gagal jantung
* Pasien yang menderita Diabetes tidak memiliki pengaruh signifikan terhadap kematian akibat gagal jantung
* Pasien yang memiliki persentase darah yang meninggalkan jantung pada setiap kontraksi dengan range 15% sampai dengan 35% memiliki resiko meninggal akibat gagal jantung
* Pasien menderita hipertensi tidak memiliki pengaruh signifikan terhadap kematian akibat gagal jantung
* Jumlah trombosit dalam darah (kiloplatelet/mL) pasien tidak memiliki pengaruh signifikan terhadap kematian akibat gagal jantung
* Pasien dengan kadar kreatinin serum dalam darah antara 0.75 (mg/dL) sampai dengan 1.0 (mg/dL) memiliki kemungkinan resiko meninggal akibat gagal jantung
* Pasien dengan kadar serum sodium dalam darah antara 120 (mEq/L) sampai dengan 140 (mEq/L) memiliki kemungkinan meninggal akibat gagal jantung
* Jenis kelamin pasien tidak memiliki pengaruh signifikan terhadap kematian akibat gagal jantung
* Pasien dengan kebiasaan merokok dan tidak memiliki kebiasaan merokok tidak memiliki pengaruh signifikan terhadap kematian akibat gagal jantung
* Pasien dengan periode tindak lanjut antara 1 sampai dengan 50 (hari) memiliki kemungkinan meninggal akibat gagal jantung 


#### Model Analysis 

Dalam menentukan model Classication yang ingin dipakai, kita membandingkan model RandomForestClassifier, AdaBoostClassifier, GradientBoostingClassifier dan melakukan evaluasi performa dari model tersebut

#### Pemilihan Model
Dari hasil perbandingan model classification tersebut dipilih model **RandomForestClassifier** karena memiliki nilai metrics tertinggi yaitu dengan nilai **Accuracy 0.78**, nilai **recall 0.57**, nilai **precision 0.84**, dan nilai **roc_auc_score 0.86**
