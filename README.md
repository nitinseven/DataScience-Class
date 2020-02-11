# DataScience-Class
Basics of Data Science with numpy, pandas and matplotlib
<code>
#Try this pie chart
import pandas as pd <br>
import matplotlib.pyplot as plt<br>
data = pd.read_csv('CarData.csv')<br>
ax=plt.subplots(1,1,figsize=(10,8))<br>
data['FuelType'].value_counts().plot.pie(explode=[0.1,0.1,0],autopct='%1.1f%%',shadow=True,figsize=(10,8))<br>
plt.title("Pie Chart %")<br>
plt.show()
