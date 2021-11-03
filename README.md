# python-data-visualization
#Forecast of infrastructure from 2020 to 2070
import pandas as pd
import matplotlib.pyplot as plt
   
Data = {'Year': [2020,2025, 2030, 2035, 2040, 2045, 2050, 2055, 2060, 2065, 2070],
        'n_kilowatt': [87.6, 88.6, 89.5, 91.4, 91.5, 92.7, 94.4, 95.2 , 96.2, 97.2, 97.8  ]
       }
  
df = pd.DataFrame(Data,columns=['Year','n_kilowatt'])
  
plt.plot(df['Year'], df['n_kilowatt'], color='red', marker='o')
plt.title('Population with access to electricity', fontsize=18,color='green')
plt.xlabel('Years 2020-2070', fontsize=14,color='blue')
plt.ylabel('percent of population', fontsize=14,color='blue')
plt.legend(['Index of access'])
plt.grid(True)
plt.show()
