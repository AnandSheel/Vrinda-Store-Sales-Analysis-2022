# Vrinda-Store-Sales-Analysis-2022

## ABOUT:
 In 2022, Vrinda stores noticed a huge set of sales. This was noticed since the store embraced online marketing at the 
 beginning of the year and the employing of a Data Analyst.

## OBJECTIVE:
 Vrinda store wants to create an annual sales report for 2022. So that, Vrinda can understand their customers and grow more sales in 2023.
 
 What can the store do better to make more sales and through what means? The task is to create an analysis and derive insights from the 2022 store sales and share them with stakeholders, so we can plan better for 2023.

### Business Questions:

• Compare the sales and orders using a single chart.
       
• Who got the highest sales and orders?

• Which month purchased more - men or women in 2022?

• What is the different order status in 2022?

• List the top 5 states that contribute to the sales.

• Relation between age and gender based on several orders.

• Which channel is contributing to maximum sales?

• Highest selling category? etc.


# DATA CLEANING

This is a full view of the dataset on my Excel worksheet


![Screenshot 2023-12-04 182050](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/6678aaa9-0cb2-44e0-91f6-3e2493bdac13)



The data cleaning begins. Create a new worksheet and copy the original information to this sheet, which will be our working sheet. In the dataset, a lot of disrupting factors can be seen. Make sure that the spelling of the header rows is accurate.

The first and most efficient way to deal with them is to apply filters across the cells. With the filters in place, we can easily see what data entries are in each row.



In the Gender column, we can see that there are misspellings for the words Men & women. This can be easily corrected with the find and replace button on the home tab.



![Screenshot 2023-12-04 182317](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/1b3e5ebf-fe22-436e-8dcf-666b45176049)

![Screenshot 2023-12-04 182447](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/62cc1c69-832b-4bf4-922f-249f5bdf70b5)

![Screenshot 2023-12-04 182516](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/8cf7c111-a9d7-40e8-ae10-f7bd3239d55e)



The outcome.



Another area to look at would be the Quantity column, the same find and replace tool would be used to correct this.



![Screenshot 2023-12-04 182827](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/75a5bde0-97c5-4cbd-9135-6e513d5ee92a)

![Screenshot 2023-12-04 182840](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/e1189f2b-c186-44bd-b2c3-9ec6d63c8f3a)




The Outcome.



![Screenshot 2023-12-04 182852](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/c95dcfc0-2b94-4579-9496-23610b8320f9)



# DATA PROCESSING

Based on two questions in our analysis report, we would have to create two new columns to help achieve this. The first would be an “age group”, so we can easily determine the sets of people in our database. This would be written using the formula below, to represent three categories “Senior, Adult, and Young”



![Screenshot 2023-12-04 160406](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/81a2aae9-2fa2-487d-b0ff-fe34c2224ee1)




The second would be the months when the sales happened. This can be solved with a small formula



![Screenshot 2023-12-04 160530](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/e7d5f2db-2388-4e0e-b6d8-5f09b07d1f3f)




With this, our data cleaning is complete and ready for us to analyze. It is important to note here that a revenue column was not included in the dataset, so a few visuals and numbers would not be easily generated.


# DATA ANALYSIS


In this section, I created my pivot tables to help analyze better. You should probably do this on a new sheet so you have more space to work with. The first question we have is to compare the sales vs orders and the second is to show the highest month. On a pivot table, I joined them to come up with a column chart, using the newly created ‘month’ column in the Row section and the ‘sum of amount and count of ID’ in the values section.


![Screenshot 2023-12-04 183659](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/c2234284-dec3-4717-a500-830edd18dc89)



The second question is to know the gender that purchased most. On the pivot table, the ‘gender’ column goes to the row, and the ‘sum of amount’ goes to the values section.

![Screenshot 2023-12-04 183813](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/baa9476d-955f-4c6a-8b1a-cf5fdf8a07eb)


The third was to show the order status of the goods at the store. The ‘status’ column would be on the Row section and the ‘orderID’ on the values section.
![Screenshot 2023-12-04 183951](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/93b6c90a-7dfd-4b46-b14d-321fa4ad919f)


Next, we have the top 5 states. To do this, we put the ‘ship-state’ column in the Row section and the ‘sum of amount’ in the Values section. Right-click on the created pivot table and select sort. Sort in descending order. Right-click on the state column and select ‘filter’, then select ‘top 10’ and you can limit or increase the number you want to set your data to. I would be going with 5 as required.


![Screenshot 2023-12-04 184046](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/08b8b4e5-5f0f-43b1-908d-bf28a8c64114)



Next would be the Age and Gender column. This is done by putting the ‘Gender’ in the column section, the ‘Age-group’ in the Rows section, and the ‘Count of OrderID’ in the Values section. Select a cell in the pivot table and right-click, select ‘show value as’, and then select % of the total.


![Screenshot 2023-12-04 184145](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/62b2d95d-f6f8-4209-9ceb-fa23201ccdae)


Finally, we have the channel category. To do this, we include the ‘Channels’ in the Row section and the ‘Count of OrderID’ in the Values section. Right-click again and select ‘show value as’, then select % of the total.
![Screenshot 2023-12-04 184404](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/269a6287-0b3f-463e-bb11-4ee1cb5e2777)



# DASHBOARD

With all our tables and charts created, we can proceed to group all of them. To do this, we create another sheet and name it ‘Dashboard’. Copy and paste all our charts into this sheet. This is the finished look of the project and what I’ll share with the stakeholders. I also added 3 slicers to help navigate and show metrics for each sub-category (Month, Channel, Category). Connect the slicers to the dashboard and this is the final look.
![Screenshot 2023-12-04 184546](https://github.com/AnandSheel/Vrinda-Store-Sales-Analysis-2022/assets/149947209/e4b01ca3-dba4-41bf-8862-566608ae9500)


# INSIGHTS

From my findings, Women were our major buyers with 65% more than men. The age group representing the Adults (30 and above) were our major buyers also. Our products sold well on the Amazon, Flipkart, and Myntra channels with Maharashtra as the top selling state. Most orders were delivered, so our delivery channel is meant to be kept the same at the moment.

Although a lot of good reports were made, to generate more sales we would have to appeal to the Male Gender. This would be from the choice of dressings sold. In 2022, most of our goods were women’s items of clothing. In 2023, we should put more sections up for the Males, and also run advertisements to let them know we’ve heard them.

Also, Senior citizens seem not to like most of our products, this may be due to them not being able to use our website/platform to order and shop for goods. A simple introductory guide for users using our platform would be useful. Ads and Coupon codes could also be used to generate sales for all age sectors.

