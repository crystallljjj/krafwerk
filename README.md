In this Amazon Coupon dataset, I focused on analyzing the "Coffee" and "bar" coupon.
The analyzing notebook is located at https://github.com/crystallljjj/krafwerk/blob/main/prompt.ipynb.

The general information of the dataset is

![image](https://github.com/crystallljjj/krafwerk/assets/14128797/6da44527-d06c-403c-aeba-4e0cd57f277d)

The general acceptance rate is 0.57

![image](https://github.com/crystallljjj/krafwerk/assets/14128797/c5d60478-a313-428d-9c67-f42af888e034)


Classify the accept coupon by the type. Restaurant(<20) and Carry out have relatively large amounts.

![image](https://github.com/crystallljjj/krafwerk/assets/14128797/33e14cff-50b5-4621-8819-635dedb975fa)

The distribution of the dataset is plot vs temperature and occupations.

![image](https://github.com/crystallljjj/krafwerk/assets/14128797/bdc418c8-fed5-41cf-9527-f207bbdc79a7)
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/589b7e37-30c7-4544-89c9-fd5793d567ba)


First session: Bar coupon analysis
1. What proportion of bar coupons were accepted?  49.9%
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/a30a1558-fbd9-41b6-9e48-bc06e82080c7)

2. Compare the acceptance rate between those who went to a bar 3 or fewer times a month to those who went more.
37.1% vs 76.9%

   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/b45c4ade-3044-47d7-90e1-2c4f52f26fcc)


4. Compare the acceptance rate between drivers who go to a bar more than once a month and are over the age of 25 to the all others. Is there a difference?
68.8% vs 38.3%

5. Use the same process to compare the acceptance rate between drivers who go to bars more than once a month and had passengers that were not a kid and had occupations other than farming, fishing, or forestry.
68.8% vs 43.3% vs 41.0%

6. go to bars more than once a month, had passengers that were not a kid, and were not widowed *OR*
   go to bars more than once a month and are under the age of 30 *OR*
   go to cheap restaurants more than 4 times a month and income is less than 50K.
   68.8% vs 72.2% vs 45.4%
   
The conclusion is:
  #### First, the frequency to go to bar in one month is a critical factor to effect whether they accept the coupon or not. Besides, age, income, marriage status and whether they have kids when drive will also affect their decisions.
  #### Based on the pre-setup quesitons above, we can have a conclusion is that  people who go to bar more than once a month and age is under 30, with no kids accompany, is approaching to accept the "Bar coupon".



Second Session: Coffee House coupon
1. What proportion of bar coupons were accepted?  49.9%
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/3bd4257e-2730-4b8e-979f-bd9ff2696855)

coffee house coupon data plot vs how often people go to coffee house
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/2114ca58-93b7-4c8e-8d6b-aa033063da75)

coffee house coupon data plot vs occupations
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/cddeb8c5-b41e-42d2-9b61-957a22e2dd36)

2. Compare the acceptance rate between those who went to a bar 3 or fewer times a month, but not never to those who went more.
56.4% vs 67.5%
People who never goes to Coffee House, has lowest acceptance rate. 18.9%

![image](https://github.com/crystallljjj/krafwerk/assets/14128797/cad39f22-3f80-48ac-9cd4-dfeb13dc0cd7)

3. Compare the acceptance rate between drivers who go to a bar more than once a month and are over the age of 25 to the all others. Is there a difference?
66.0% vs 48.1%

4. Use the same process to compare the acceptance rate between drivers who go to coffee house more than once a month and had passengers with 'Friends' and had occupations are 'Student' and 'Computer & Mathmatic'.
66.0% VS 57.9%% vs 58.1%

5.  Compare the acceptance rates between those drivers who:
  go to bars more than once a month, had passengers were friends, and were not widowed *OR*
  go to bars more than once a month and are under the age of 25 *OR*
  go to restaurants 20 ~50 more than 4 times a month and income is less than 50K.
  76.3% vs 71.3% vs 68.7%
Conclusion:
    #### The acceptance of "Coffee coupon" are affected a lot by people's life style, for example, how often they go to coffee house, how much they are willing to spend on restaurant. They also varies based on occupation and income.
    #### Based on previous results, it shows that people used to go to coffee house more than once a month, under 25 and go to restaurant20To50 more than 3 times a month is more likely to accept the coupon. Besides, people with occupation as 'Student' and 'Computer & Mathematical' are more likely to accept coupon. In addition, when the driver is with friends, are more likely to accept the coupon.
  
  #### recommendation: Based on the data, overall, the cheap restaurant and carry out shows large possibility to accept the coupon. Focus on these people, more accurate to send the coupon will improve the efficiency. For other classes, like Bar, Coffee House and Restaurant(20-50) are more likely bonded with the living style of the people. To imrpve the coupon acceptance, the company may classify the coupon in different group of people. Those people may live in different areas. Like, the coffee house coupon could focus on IT working area and school area. 

