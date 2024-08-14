## 1. Dataset Description
The dataset **athletes.xlsx** contains various information about the athletes participating in the Paris 2024 Olympic Summer Games.


## 2. Preliminary Data Cleaning (Power Query)
Firstly, we will remove the athlete name columns: **name**, **name_short** and **name_tv**; as these columns are unlikely to provide interesting insights.

![athlete name columns](.\Images\AD1.PNG)

The column **function** contains only two categories: Alternate Athlete and Athlete. Again, not much insight could be extracted from this column, hence, we should remove this column as well.

![function column](.\Images\AD2.PNG)

Next, we will remove the **country_code** and **country** columns, and use **country_full** column to represent the country that each athlete represents.

![country columns](.\Images\AD3.PNG)

Since we have the **country_full** column to represent the countries, we are unlikely to need the **nationality**, **nationality_full**, and **nationality_code** columns. Therefore we should delete these columns.

![nationality columns](.\Images\AD4.PNG)

Next, we will change the data type of the **height** and **weight** to whole numbers, so that we could use these columns for data analysis.

![height and weight columns](.\Images\AD5.PNG)

The column **disciplines** contains symbols that will be difficult for visualisation, therefore we will remove those symbols.

![disciplines columns](.\Images\AD6.PNG)

![disciplines columns](.\Images\AD7.PNG)

Since we have the **disciplines** column, thus, we are unlikely to need the **events** column.

![disciplines columns](.\Images\AD8.PNG)

For simplicity, we will use the year from the **birth_date** column to calculate the age of the athletes. 

![disciplines columns](.\Images\AD9.PNG)

We will first extract the year from the **birth_date** column.

![disciplines columns](.\Images\AD10.PNG)

Then, we will create a new column called **age** that calculates the age of the athletes by subtracting the extracted year from 2024.

![disciplines columns](.\Images\AD11.PNG)


Lastly, we will delete the columns **birth_place**, **birth_country**, **residence_place**, **residence_country**, **nickname**, **hobbies**, **occupation**, **education**, **family**, **lang**, **coach**, **reason**, **hero**, **influence**, **philosophy**, **sporting_relatives**, **ritual**, and **other_sports**. As these columns are either irrelevant or contain messy data that are hard to work with.