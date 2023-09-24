# ShipTimeForecasters Shoppedia e-commerce Shipping Data Project

Project Title: Shipping Forecasting for Shoppedia e-commerce. \
Project Goal: to increase Delivery on Time rate from 40% to 60%.\
Project Objective: to predict whether the packages from Shoppedia e-Commerce company arrived on time or not based on the historical dataset.\
Dataset: ID, Warehouse Block, Mode of Shipment, Customer care calls, Customer ratings, Cost of the Product, Prior purchases, Product importances, Gender, Discount offered, and Weight. \
Insight summary:
1. High Discounts correlate positively with Late Deliveries.
2. Weight and Price of Products impact Timely Deliveries.
3. Warehouse Blocks and Mode of Shipment Affect Discounts and On-Time Deliveries.

Data Preprocessing Summary:
1. Tidak terdapat missing value, duplicate data, dan invalid value.
2. Dilakukan feature extraction dengan nama Weight_class dari feature berat barang (Weight_in_gms), menjadi 4 kategori berdasarkan beratnya.
3. Dilakukan feature selection berdasarkan multicolinearity, variance dan entropy, dan Information Value. Feature yang masih digunakan yaitu Customer_care_calls, Cost_of_the_Product, Discount_offered, Prior_purchases, Product_importance, dan Weight_class.
4. Dilakukan train/test data split untuk persiapan machine learning modeling. 
5. Tidak dilakukan handling outlier karena dataset yang kecil, transformasi data menggunakan metode yang robust terhadap outlier.
6. Transformasi dan scaling data dilakukan pada feature Cost_of_the_Product dan Discount_offered.
7. Dilakukan Label Encoding untuk Feature Encoding untuk feature kategorikal (Product_importance).
8. Tidak dilakukan handling class imbalance, karena jumlah nilai pada dataset tidak masuk dalam kriteria class imbalance. 
