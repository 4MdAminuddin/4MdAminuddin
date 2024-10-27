import matplotlib.pyplot as plt
import pandas as pd
df=pd.read_csv('data.csv')
df.head()
max_values=df.max()
avg_scores = df.groupby('gender')[['math score', 'reading score', 'writing score']].mean()
avg_scores.plot(kind='bar')
plt.title("Average Scores by Gender")
plt.show()

df=pd.DataFrame(data.csv)
print(df.isnull())
avg_scores = df.groupby('parental level of education')[['math score', 'reading score', 'writing score']].mean()
avg_scores.plot(kind='bar')
plt.title("Average Scores by Parental Education")
plt.xticks(rotation=45)
plt.show()

avg_scores = df.groupby('lunch')[['math score', 'reading score', 'writing score']].mean()
avg_scores.plot(kind='bar')
plt.title("Average Scores by Lunch Type")
plt.show()

avg_scores = df.groupby('test preparation course')[['math score', 'reading score', 'writing score']].mean()
avg_scores.plot(kind='bar')
plt.title("Average Scores by Test Preparation Course")
plt.show()
