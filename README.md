# EXNO5APPDS

# AIM:

      To implement Dashboards creation with Plotly and Dash using python.
      

# About Dash and Plotly tools:

Dash is a Python framework for building analytical web applications. Dash helps in building responsive web dashboards that is good to look at and is very fast without the need to understand complex front-end frameworks or languages such as HTML, CSS, JavaScript. Let’s build our first web dashboard using Dash.

Plotly library in Python is an open-source library that can be used for data visualization and understanding data simply and easily. Plotly supports various types of plots like line charts, scatter plots, histograms, box plots, etc.


# ALGORITHM:

Step 1: Import Necessary Library like dash and plotly.

Step 2: Load the dataset.

Step 3: Add dropdown using layout function and include the necessary options.

Step 4: Display the necessary visualization tools and include the necessary parameters.

Step 5: Display the output.


# CODING AND OUTPUT:
```c
pip install dash plotly pandas
import dash
from dash import dcc, html
from dash.dependencies import Input,Output
import plotly.express as px
import pandas as pd
import plotly.graph_objects as px
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df = sns.load_dataset('tips')

```
![386476853-ee82fe00-e367-458e-8c75-698571c62065](https://github.com/user-attachments/assets/7ec20fa8-13dd-4c19-8379-3e0b6633321f)


```c
import plotly.express as px
df=px.data.tips()fig = px.scatter_3d(df, x="total_bill",y="sex",z="tip",color='day',size='total_bill',symbol='time')
fig.show()

```

![386476939-bd19fa83-f3a8-4fe4-8132-2477ef9f4631](https://github.com/user-attachments/assets/b0a3bfb3-db95-4f5d-b07b-2d9c410f3b36)


```c
import plotly.express as px
df=px.data.tips()
fig = px.bar(df, x='day',y='total_bill',color='sex',facet_row='time',facet_col='sex')
fig.show()
```


![386477178-1ee7ce0e-1bd1-4913-a701-a8b71e6bb006](https://github.com/user-attachments/assets/ed88a7d1-c646-4c3d-94ad-ab0e78ecd096)

```c
import plotly.express as px
df=px.data.tips()
fig = px.histogram(df, x='total_bill',color='sex',nbins=50,histnorm='percent',barmode='overlay')
fig.show()

```
![386477263-625816bf-3409-4e0b-b5e0-3f08f70c34b6](https://github.com/user-attachments/assets/40860be0-36ae-4e56-bc9d-d8544ad6cfb8)

```c
import plotly.express as px
df=px.data.tips()
fig = px.pie(df, values='total_bill',names='day')
fig.show()


```


![386477344-96ba396c-85bc-454d-81e3-d68310903377](https://github.com/user-attachments/assets/c995d90b-ca77-4df1-a9ff-d1e007648e5e)

# RESULT:

Thus , To implement Dashboards creation with Plotly and Dash using python is successfully done.

