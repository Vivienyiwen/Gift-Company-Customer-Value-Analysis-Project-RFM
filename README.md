# RFM

Project Source:
https://www.kaggle.com/carrie1/ecommerce-data

Project Description:
This is a cross-country dataset of all online retail transactions that occurred between December 1, 2010 and December 9, 2011 for stores registered in the United Kingdom. The company mainly sells unique all-day gifts and many of its customer targets are wholesalers.

The main objective of this project is to use the RFM model for user classification.



### Import Modules
<img width="1044" alt="image" src="https://user-images.githubusercontent.com/97607988/178101189-bb213254-1ff2-42d9-a7e2-37e24c028124.png">

### Load Data
<img width="1042" alt="image" src="https://user-images.githubusercontent.com/97607988/178101232-b0192943-9a6c-4608-bef5-a44cce6e25e5.png">

### Data exploration and data cleaning

1.Data exploration
<img width="1057" alt="image" src="https://user-images.githubusercontent.com/97607988/178101305-92eb08d8-af19-4d4f-a64b-46abffb361a7.png">

<img width="1049" alt="image" src="https://user-images.githubusercontent.com/97607988/178101325-4f765a75-5b9a-4d64-a05f-bbccfd2f4a5a.png">
It can be seen that we need to perform date format conversion, as well as the usual missing value statistics, de-duplication, and outlier detection and processing.

2.Missing value statistics
<img width="942" alt="image" src="https://user-images.githubusercontent.com/97607988/178101356-b563498f-d857-4a9b-b1e6-c3a545fbf012.png">

3.Date format conversion
<img width="1051" alt="image" src="https://user-images.githubusercontent.com/97607988/178101392-8171f271-a26f-40ad-8c74-680487ebcbae.png">

4.de-duplication
<img width="1058" alt="image" src="https://user-images.githubusercontent.com/97607988/178101415-b68da8ea-e334-4796-9fe0-04ea5197636b.png">

5.Outlier handling
<img width="1064" alt="image" src="https://user-images.githubusercontent.com/97607988/178101445-072895b5-b734-43d8-8c3f-1a5484fdfc3f.png">
<img width="1057" alt="image" src="https://user-images.githubusercontent.com/97607988/178101458-f4dccde2-a40b-44e7-ad06-840600588b3c.png">

### User Classification

1.Calculate R-value
<img width="1057" alt="image" src="https://user-images.githubusercontent.com/97607988/178101484-c7a2e109-944a-47d8-a00f-193b76ece3c0.png">
2.Calculate F-value
<img width="1063" alt="image" src="https://user-images.githubusercontent.com/97607988/178101498-d6cf4ffb-ff49-420a-9d9d-b42044a07fbe.png">
3.Calculate M-value
<img width="1066" alt="image" src="https://user-images.githubusercontent.com/97607988/178101541-13c53bde-ffd3-4376-b28a-c635cd4efda2.png">

<img width="1055" alt="image" src="https://user-images.githubusercontent.com/97607988/178101585-6022b7d6-c9b0-4bbe-bcb1-c6cd0c5ffab4.png">
<img width="1055" alt="image" src="https://user-images.githubusercontent.com/97607988/178101597-45a3f3e5-d0f1-4b50-b6f7-f74f10b2b257.png">

<img width="1057" alt="image" src="https://user-images.githubusercontent.com/97607988/178101602-2676be3e-db26-4b28-9ac6-8f930807a797.png">
<img width="1054" alt="image" src="https://user-images.githubusercontent.com/97607988/178101613-2f610069-8840-4998-82a6-eaf3ef0bb619.png">
<img width="1058" alt="image" src="https://user-images.githubusercontent.com/97607988/178101623-a758bab5-35d1-4592-bdeb-d27d43d38ad7.png">
It can be seen that the data are very unevenly distributed

<img width="1049" alt="image" src="https://user-images.githubusercontent.com/97607988/178101653-0fcd7433-aee6-46e5-87b4-88bac1d3650f.png">

<img width="1056" alt="image" src="https://user-images.githubusercontent.com/97607988/178101662-093dffa2-fd33-4d81-a269-4936278de07d.png">
<img width="1057" alt="image" src="https://user-images.githubusercontent.com/97607988/178101670-b7823037-dd4f-4e1c-bf68-8860b63bb662.png">
<img width="1053" alt="image" src="https://user-images.githubusercontent.com/97607988/178101674-c8eba7c3-9138-4d88-8dd1-1e1ccef2f02c.png">
<img width="1054" alt="image" src="https://user-images.githubusercontent.com/97607988/178101677-7cc2815b-730c-4c68-9fee-5cab6b011231.png">
All the same, it is very uneven.

<img width="1059" alt="image" src="https://user-images.githubusercontent.com/97607988/178101706-26be1991-6960-48ed-a8c8-5dc618236c47.png">
R
<img width="1053" alt="image" src="https://user-images.githubusercontent.com/97607988/178101719-efc0e6b0-3114-4469-80d6-a68269b2eafb.png">

F
<img width="1054" alt="image" src="https://user-images.githubusercontent.com/97607988/178101731-b1f578e5-dd0e-4fbe-abe0-1727d7fe790b.png">

M
<img width="1058" alt="image" src="https://user-images.githubusercontent.com/97607988/178101739-2892a021-e2c3-4900-911d-3d8e920fab26.png">

Generate a new data frame.
<img width="1057" alt="image" src="https://user-images.githubusercontent.com/97607988/178101753-e283ec16-f023-43f0-9f62-22e60705059b.png">
<img width="1059" alt="image" src="https://user-images.githubusercontent.com/97607988/178101822-28423f09-703c-40e7-9c46-d4508ec4da40.png">

Change the data format
<img width="1060" alt="image" src="https://user-images.githubusercontent.com/97607988/178101826-c6507256-5025-4c83-836b-7ee04af70a05.png">

High(高) and low(低) values by mean under each indicator
<img width="1052" alt="image" src="https://user-images.githubusercontent.com/97607988/178101843-8a99b08c-46f7-429f-992a-c92d59779207.png">

Combining the three indicators
<img width="1062" alt="image" src="https://user-images.githubusercontent.com/97607988/178101873-a1e44c7e-9a8c-4581-9d78-917ec49b2ac4.png">

<img width="1055" alt="image" src="https://user-images.githubusercontent.com/97607988/178101890-2e39b0b4-517b-4eb4-ab99-963bb158541f.png">
<img width="630" alt="image" src="https://user-images.githubusercontent.com/97607988/178101899-3f8f4c3f-7476-4ad8-b298-69576e690d72.png">

### Classification results
<img width="1066" alt="image" src="https://user-images.githubusercontent.com/97607988/178101920-41928503-58d3-4571-941d-13c40d4fa54e.png">

<img width="933" alt="image" src="https://user-images.githubusercontent.com/97607988/178101929-af44f55f-c2ab-407d-af0d-e1a5e3d3390f.png">
<img width="1060" alt="image" src="https://user-images.githubusercontent.com/97607988/178101945-47ba96e8-42e5-4871-89a7-1d299d5ff7a8.png">

<img width="1056" alt="image" src="https://user-images.githubusercontent.com/97607988/178101955-c41f7d85-65c4-475a-8a61-be34e968989e.png">
<img width="877" alt="image" src="https://user-images.githubusercontent.com/97607988/178101960-635d0f8d-8a82-493e-8f6f-1f736bc6edc3.png">

### Conclusions and Recommendations

The results of the user classification percentage show that high-value customers and important development customers, which together account for 47% of the total, are an important source of revenue for the company.

High-value Customers（111）（高高高）
All three values of RFM are high and should be offered vip services to them.

Key Customers for development（101）（高低高）
Consumption frequency is low, but the other two values are very high, we must find ways to improve his consumption frequency, it is recommended that timely push the company's activity information or new product-related information to attract customers.

Key Retention Customers（011）（低高高）
The recent consumption is far from the present time, that is, the F value is low, but the consumption frequency and consumption amount is high. This kind of user is a loyal customer who has not come for some time. Should take the initiative to keep in touch with him to increase the repurchase rate. Coupons can be given or product discounts can be pushed to increase the number of purchases.

Key Retained Customers（001）（低低高）
Recent consumption time is far away from now, low consumption frequency, but high consumption amount. Such users, about to lose, should take the initiative to contact the user, investigate what went wrong, and find ways to recover. Of course the same can be done by giving coupons or pushing information about product discounts to increase the number of purchases.

General Development Clients（100）（高低低）
The company should obtain detailed data and user profiles of customers to understand their consumption attributes. It is recommended that such customers should be marketed precisely and product information should be pushed in a timely manner.

The final marketing strategy should be determined based on the company's own financial commitment.

RFM should also not be overused and cause high transaction customers to keep receiving letters. Each company should design a customer contact frequency rule, such as within three days or a week of purchase should send a thank you call or Email, and proactively care about whether consumers have problems with the use of the consumer, a month later send an inquiry whether the use is satisfactory, while three months later provide cross-selling advice, and begin to pay attention to the possibility of losing customers, and constantly create opportunities to proactively contact customers. In this way, the chances of customers buying again will also increase dramatically.High-value CustomersHigh-value Customers.
