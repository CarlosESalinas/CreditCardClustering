<center> <h1> Credit Card: K-Means Clustering</h1> </center>

<br>
<center>
<img src="https://static.toiimg.com/thumb/66538171.cms?resizemode=4&width=400"></center>
source image: https://bangaloremirror.indiatimes.com/bangalore/others/credit-card-customer-walks-away-bank-loses-rs-30000-it-didnt-have-record-of-his-application/articleshow/66538133.cms

<h3> Summary </h3>

Credit card segmentation is a crucial strategy used by financial institutions to categorize their customers based on various attributes and behaviors. This practice allows banks and credit card companies to better understand their customer base, tailor their products and services to specific groups, and optimize marketing efforts.

The importance of credit card segmentation lies in its ability to provide personalized solutions and offers to different customer segments. By identifying distinct groups of customers with similar needs and spending patterns, banks can create targeted marketing campaigns, loyalty programs, and rewards that are more likely to resonate with each segment. This, in turn, enhances customer satisfaction and increases the likelihood of customer retention.

<h3> Statement of the problem and goal </h3>

Since the data are collected by every credit activities, the company hope they could get some insight by processing the data. This time, we have a data contains summary of the usage behavior of about 9000 active credit card holders during the last 6 months. We will process this data using unsupervised learning methodology to segmentize the customer by finding a certain pattern in hope we could find some characteristic between each customer segment.

Then we will analyze each segment and plan the marketing approach that work best with each segment. We also give some recommendation for the next if we want to update the model or strategies.


## Dataset

The data set was obtained from the following <a href = "https://www.kaggle.com/datasets/arjunbhasin2013/ccdata">link. </a>
> <i>The sample Dataset summarizes the usage behavior of about 9000 active credit card holders during the last 6 months. The file is at a customer level with 18 behavioral variables.</i>
    

Following is the Data Dictionary for Credit Card dataset :

<table class="default">
  <tr>
    <th>Variable</th>
    <th>Description</th>
 </tr>
 <tr>
    <td><b>CUST_ID</b></td>
    <td>Identification of Credit Card holder (Categorical)</td>
 </tr> 
 <tr>
    <td><b>BALANCE</b></td>
    <td>Balance amount left in their account to make purchases.</td>
</tr>
<tr>
    <td><b>BALANCE_FREQUENCY</b></td>
    <td>How frequently the Balance is updated, score between 0 and 1 (1 = frequently updated, 0 =         not frequently updated)</td>
</tr>
<tr>
    <td><b>PURCHASES</b></td>
    <td>Amount of purchases made from account.</td>
</tr>
<tr>
    <td><b>ONEOFF_PURCHASES</b></td>
    <td>Maximum purchase amount done in one-go.</td>
</tr>
<tr>
    <td><b>INSTALLMENTS_PURCHASES</b></td>
    <td>Amount of purchase done in installment.</td>
</tr> 
<tr>
    <td><b>CASH_ADVANCE</b></td>
    <td>Cash in advance given by the user.</td>
</tr> 
<tr>
    <td><b>PURCHASES_FREQUENCY</b></td>
    <td>How frequently the Purchases are being made, score between 0 and 1 (1 = frequently
        purchased, 0 = not frequently purchased).</td>
</tr> 
<tr>
    <td><b>ONEOFFPURCHASESFREQUENCY</b></td>
    <td>How frequently Purchases are happening in one-go (1 = frequently purchased, 0 = not
        frequently purchased).</td>
</tr> 
 <tr>
    <td><b>PURCHASESINSTALLMENTSFREQUENCY</b></td>
    <td>How frequently purchases in installments are being done (1 = frequently done, 0 = not
        frequently done).
</td>
</tr> 
<tr>
    <td><b>CASHADVANCEFREQUENCY</b></td>
    <td>How frequently the cash in advance being paid.
</td>
</tr> 
<tr>
    <td><b>CASHADVANCETRX</b></td>
    <td>Number of Transactions made with "Cash in Advanced".
</td>
</tr> 
<tr>
    <td><b>PURCHASES_TRX</b></td>
    <td>Numbe of purchase transactions made.
</td>
</tr> 
<tr>
    <td><b>CREDIT_LIMIT</b></td>
    <td>Limit of Credit Card for user.</td>
</tr> 
<tr>
    <td><b>PAYMENTS</b></td>
    <td>Amount of Payment done by user.
</td>
</tr> 
 <tr>
    <td><b>MINIMUM_PAYMENTS</b></td>
    <td>Minimum amount of payments made by user.
</td>
</tr> 
<tr>
    <td><b>PRCFULLPAYMENT</b></td>
    <td>Percent of full payment paid by user.
</td>
</tr> 
<tr>
    <td><b>TENURE</b></td>
    <td>Tenure of credit card service for user.</td>
</tr> 
</table>

