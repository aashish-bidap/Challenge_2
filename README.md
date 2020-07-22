**Django Challenge Documentation:**

Write a simple application that allows a user to manage subscriptions using Stripe and Python Django 2.

**Functional Flow :**

**1.Old Users can Login / New Users registration.**

![](/Picture1.png)

![](/Picture2.png)

**2.Once the user registration is through :**

**1. User profile in Django will be created with attributes**

**1.User**

**2.StartDate - Subscription start date**

**3.Free\_trial = 7**

**4.Free\_trialEndDate = Subscription start date + free trial**

**2. Customer would be created on Stripe and assigned with a membership of 49.99 and a free trial of 7 days.**

![](/Picture3.png)

**3. Stripe subscription would be assigned to the subscriber with**

**1. plan id which is pre created with charge of 49.99**

**2. payment method= &quot;send invoice&quot;**

**3.Due date for the invoice is assumed to be 10**

![](/Picture4.png)

**3.User Profile View with Account Details after login into the account**

![](/Picture5.png)

- **Customer can cancel the membership here:**

![](/Picture6.png)

**After Cancellation Django Profile:**

![](/Picture7.png)

**States of Customer:**

**Active : Customer successfully registers for the membership.**

**Active Canceled : membership would remain active till the end of billing period.**

**Inactive: after the end of billing period.**

**After Cancellation Stripe Profile:**

![](/Picture8.png)