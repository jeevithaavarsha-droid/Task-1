import pandas as pd
import matplotlib.pyplot as plt

# Load dataset
data = pd.read_csv("Students Social Media Addiction.csv")

# Histogram for Age
plt.hist(data["Age"], bins=10)
plt.title("Age Distribution")
plt.xlabel("Age")
plt.ylabel("Number of Students")
plt.show()

# Bar chart for Gender
data["Gender"].value_counts().plot(kind="bar")
plt.title("Gender Distribution")
plt.xlabel("Gender")
plt.ylabel("Number of Students")
plt.show()

