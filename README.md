# Cryptocurrencies
---

The purpose of this analysis is to assist an Investment Banking client who is interested in entering the world of cryptocurrencies. The investment bank would like to offer a cryptocurrency investment portfolio, but needs assistance in understanding what cryptocurrencies are on the trading market and how they could be grouped to create a classification system. Using unsupervised machine learning, I was able to analyze cryptocurency data from CryptoCmpare and begin clustering/classifying the various cryptocurrencies. Unsupervised machine learning models were used in this analysis because the data is large and the outputs aren't known.

- The first step was to load the data from the csv and clean it before clustering. In this case, I kept all cryptocurrencies in the DataFrame that were being traded, had a working algorithm, and were being mined. This resulted in a total of 532 cryptocurrencies remaining.

- The data was then standardized with StandardScaler and then I used Principal Component Analysis (PCA) to transform the data into 3 main components. 

![pca](https://github.com/AndrewTymkiv/Cryptocurrencies/blob/main/screenshots/pca.PNG)


- After the PCA was performed, the next step was to create an elbow curve to identify the number of KMeans which was k=4. This means there were 4 different clusters.

![elbow_curve](https://github.com/AndrewTymkiv/Cryptocurrencies/blob/main/screenshots/elbow_curve.PNG)


- To visualize these clusters of cryptocurrencies, a 3D graph was created to show how they all cluster and classify, with most cryptocurrencies being in one of two different clusters. 

![3D](https://github.com/AndrewTymkiv/Cryptocurrencies/blob/main/screenshots/3D.PNG)


- A table with sorting abilities was also created to provide a simpler way to view data for any individual cryptocurrency. 

![table](https://github.com/AndrewTymkiv/Cryptocurrencies/blob/main/screenshots/table.PNG)


- The last visualization created was a 2D scatter plot to show the relationship between the Total Coins Mined (x) and the Total Coins in Supply (y).

![2D](https://github.com/AndrewTymkiv/Cryptocurrencies/blob/main/screenshots/2D.PNG)
