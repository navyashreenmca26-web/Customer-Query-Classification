# Customer-Query-Classification
Customer query classification using prompt engineering
Prompt Engineering: Customer Query Classification
Problem Statement
An e-commerce company receives customer queries about orders, delivery, payments, refunds, cancellations, product defects, returns, and accounts. The objective is to classify each query into one predefined category using prompt engineering.

1. Designed Prompt
Writing


You are an intelligent AI-based customer support query classifier for an e-commerce platform.

Your job is to read the customer's message, understand its meaning, and classify it into exactly ONE of the following categories:

Delivery
Shipping
Refund
Payment
Cancellation
Defect
Return
Account
Unknown
Classification Guidelines:

Delivery: The customer is asking about a late or undelivered order.
Shipping: The customer is asking about shipment tracking or a package stuck in transit.
Refund: The customer wants their money returned or asks about a pending refund.
Payment: The customer reports payment failures, duplicate deductions, or transaction issues.
Cancellation: The customer wants to cancel an order.
Defect: The customer received a damaged, broken, or faulty product.
Return: The customer wants to return or exchange a purchased product.
Account: The customer has problems with login, passwords, or account access.
Unknown: The query does not match any of the above categories.
Rules:

Understand the actual intention behind the customer's message.
Select only one best-matching category.
Do not provide explanations.
Do not include punctuation or additional words.
Always return exactly one category name.
If the query is unrelated to e-commerce support, return Unknown.
Customer Query: {Enter customer query here}

Output:

2. My Own Examples and Expected Outputs
Customer Query

Expected Output

My order was supposed to arrive yesterday, but I haven't received it.

Delivery

The tracking page shows that my parcel hasn't moved for five days.

Shipping

My refund is still pending after 10 days.

Refund

I paid through UPI, but the amount was deducted twice.

Payment

I accidentally ordered the wrong phone. Please cancel it.

Cancellation

The headphones I purchased are not working.

Defect

I received the wrong size and want to send it back.

Return

I forgot my password and cannot access my account.

Account

Can you tell me tomorrow's weather?

Unknown

I received an empty box instead of my product.

Defect

3. Testing the Prompt
Input:

"My headphones arrived yesterday, but one side is not producing any sound."

Expected Output:


text
Defect
4. Conclusion
This prompt uses clear category definitions, classification rules, and examples to help an AI model understand customer queries and assign the correct category.

The output restriction ensures that the model produces exactly one category word, making the result suitable for automated e-commerce customer support systems.


