**Django Application Documentation:**

An application that allows a user to manage subscriptions using Stripe and Python Django 2.

**DEMO EXECUTION - Click below on the Video** <br>
<div align="center">
      <a href="https://youtu.be/tEorn2Kkwb4">
     <img 
      src="https://img.youtube.com/vi/tEorn2Kkwb4/0.jpg" 
      alt="Everything Is AWESOME" 
      style="width:100%;">
      </a>
    </div>


**Functional Flow :**

**1.Old Users can Login / New Users registration.**

![](https://github.com/aashish-bidap/Challenge_2/blob/master/Screenshots/Picture1.png)

![](https://github.com/aashish-bidap/Challenge_2/blob/master/Screenshots/Picture2.png)

**2.Once the user registration is through :**

* A User profile would be created in Django with attributes :

  * 1.User

  * 2.StartDate - Subscription start date

  * 3.Free\_trial = 7

  * 4.Free\_trialEndDate = Subscription start date + free trial

**3.Customer would also be created on Stripe and assigned with a membership of $49.99 and a free trial of 7 days.**

![](https://github.com/aashish-bidap/Challenge_2/blob/master/Screenshots/Picture3.png)

**4. Stripe subscription would be assigned to the subscriber with**

* plan id which is pre created with charge of 49.99

* payment method= send invoice

* Due date for the invoice is assumed to be 10

![](https://github.com/aashish-bidap/Challenge_2/blob/master/Screenshots/Picture4.png)

**5.User Profile View with Account Details for the customer after login into the account**

![](https://github.com/aashish-bidap/Challenge_2/blob/master/Screenshots/Picture5.png)

- **Customer can cancel the membership here:**

![](https://github.com/aashish-bidap/Challenge_2/blob/master/Screenshots/Picture6.png)

**After Cancellation Django Profile:**

![](https://github.com/aashish-bidap/Challenge_2/blob/master/Screenshots/Picture7.png)

**States of Customer:**

* Active : Customer successfully registers for the membership.

* Active Canceled : membership would remain active till the end of billing period.

* Inactive: after the end of billing period.

**After Cancellation Stripe Profile:**

![](https://github.com/aashish-bidap/Challenge_2/blob/master/Screenshots/Picture8.png)
