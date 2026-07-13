from google.colab import files
uploaded = files.upload()
import pandas as pd
import csv
import io
df = pd.read_csv(io.BytesIO(uploaded['arms_transfers_clean.csv']))
df.head(
