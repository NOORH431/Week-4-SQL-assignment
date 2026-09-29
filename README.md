# Week-4-SQL-assignment

q1.
SELECT paymentDate, SUM(amount) AS totalAmountPaid
FROM payments
GROUP BY paymentDate
ORDER BY paymentDate DESC
LIMIT 5;

q2.
SELECT customerName, country, AVG(creditLimit) AS averageCreditLimit
FROM customers
GROUP BY customerName, country;


q3.
SELECT productCode, quantityOrdered, SUM(priceEach * quantityOrdered) AS totalPrice
FROM orderdetails
GROUP BY productCode, quantityOrdered;

q4.
SELECT checkNumber, MAX(amount) AS highestAmountPaid
FROM payments
GROUP BY checkNumber;
