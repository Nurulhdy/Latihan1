# Latihan1

Kelas Data Sains

#Persentase penggunaan voucher

#Mengimport library
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn import datasets

import pandas as pd
import io

from google.colab import file
uploaded = file.upload()

df = pd.read_cvs('food_delivery_datasets')
print(df)

df_voucher = df["voucher_amount"]
df_voucher.head()

df_voucher_uses = df[df["voucher_amount"]>0]
df_voucher_uses.head()

pers = len(df_voucher_uses)*100/len(df_voucher)
print("persentase dari banyaknya pengguna voucher adalah "+str(pers))
persentase dari banyaknya pengguna voucher adalah 15.041782729805014

Dari data tersebut dapat disimpulkan bahwa persentase dari banyak custemer yang menggunakan voucher untuk pemesanan makanan sebesar 15.041782729805014 atau bisa dibulatkan menjadi 15%. Hal ini berarti masih terbilang sedikit custemer yang menggunakan voucher makanan.
