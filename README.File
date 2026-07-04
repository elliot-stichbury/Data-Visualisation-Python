# Data-Visualisation-Python

import pandas as pd
from matplotlib import pyplot as plt
sample_data = pd.read_csv('sample_data.csv')
data = pd.read_csv('countries.csv')

# Compare the population growth in the US and China

us = data[data.country == "United States"]
china = data[data.country == "China"]

# Compares population in the Us and China in millions per year

plt.plot(us.year, us.population / 10**6, 'x')
plt.plot(china.year, china.population / 10**6, '.')
plt.legend(["United States", "China"])
plt.xlabel("Year")
plt.ylabel("Population in millions")
plt.show()

# Compares percentage population increase in the US and China per year

plt.plot(us.year, us.population / us.population.iloc[0] * 100, 'x')
plt.plot(china.year, china.population / china.population.iloc[0] * 100, '.')
plt.legend(["United States", "China"])
plt.xlabel("Year")
plt.ylabel("Population growth, first year = 100")
plt.show()
