# Latihan1

Kelas Data Sains

#Persentase penggunaan voucher

import pandas as pd
import io

from google.colab import file uploaded = file.upload()

df = pd.read_cvs('food_delivery_datasets')
print(df)

df_voucher = df["voucher_amount"]
df_voucher.head()

df_voucher_uses = df[df["voucher_amount"]0]
df_voucher_uses.head()

pers = (len(df_voucher)/(df_voucher_uses))*100%

print("persentase dari banyaknya pengguna voucher adalah "+str(pers))
persentase dari banyaknya pengguna voucher adalah [0,19330855]

Dari data tersebut dapat disimpulkan bahwa persentase dari banyak custemer yang menggunakan voucher untuk pemesanan makanan sebesar 0,19330855. Hal ini berarti masih terbilang sedikit custemer yang menggunakan voucher makana.
