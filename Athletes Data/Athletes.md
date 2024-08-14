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

![country columns](.\Images\AD4.PNG)

