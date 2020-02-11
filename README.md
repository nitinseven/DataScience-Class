# DataScience-Class
Basics of Data Science with numpy, pandas and matplotlib
<code>
#Try this pie chart
import pandas as pd
import matplotlib.pyplot as plt
data = pd.read_csv('CarData.csv')
ax=plt.subplots(1,1,figsize=(10,8))
data['FuelType'].value_counts().plot.pie(explode=[0.1,0.1,0],autopct='%1.1f%%',shadow=True,figsize=(10,8))
plt.title("Pie Chart %")
plt.show()
