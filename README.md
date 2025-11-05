> 💡 **Note:**
> The file path used in the notebook corresponds to my personal Google Drive structure when mounted in Google Colab:
>
> ```python
> from google.colab import drive
> import pandas as pd
>
> drive.mount('/content/drive/')
> df = pd.read_excel("/content/drive/MyDrive/Colab Notebooks/Adidas US Sales Datasets.xlsx", header=4, parse_dates=['Invoice Date'])
> df = df.drop(df.columns[0], axis=1)
> df.info()
> ```
>
> If you’re running this notebook on your own environment, **please update the file path** according to your own folder structure or storage location.
> For example:
>
> ```python
> df = pd.read_excel("path_to_your_folder/Adidas US Sales Datasets.xlsx", header=4, parse_dates=['Invoice Date'])
> ```
>
> Make sure the dataset file is available in the specified path before executing the cell.
