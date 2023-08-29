# Schema
![schema](https://github.com/Aakaaaassh/SQL/assets/66636545/e3f0f84f-46a6-4d33-8c50-99fbe6838602)

## Practical Exam: Insurance Upgrades
<p>Travel Assured provides travel services to its customers. They are based in the United States.</p>
<p>Travel Assured provides everything from flights and hotel bookings to holiday insurance.</p>
<p>The sales team wants to sell upgrades to customers. So they can do this, it is vital that the data is clean, accurate and available for reporting. </p>
<p>They need your help to prepare some data before they start to run a new promotion. </p>
<p>The data you need is in the database named <code>insurance</code>. </p>
<p><strong>Database Schema</strong></p>
<h2 id="task1">Task 1</h2>
<p>The sales team want to use customer information to target their new promotion. But, they think the data may not be clean enough to use. The table below shows what the sales team expect the data types and format to be.</p>
<table>
<thead>
<tr>
<th>Column Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>customer_id</td>
<td>Unique integer (set by the database, can’t take any other value)</td>
</tr>
<tr>
<td>location</td>
<td>State names as a lower case string</td>
</tr>
<tr>
<td>age</td>
<td>Integer value giving age of customer</td>
</tr>
<tr>
<td>registration_date</td>
<td>Date of first registration with company (YYYY-MM-DD)</td>
</tr>
</tbody>
</table>
<p>Write a query to ensure that the <code>customer</code> table matches the description provided. </p>

## Task 2
<p>You have been informed that there has been a problem in the data entry. Some people who bought a new policy had their purchase type set to NULL instead of New.</p>
<p>Return the corrected <code>purchase</code> table.</p>

## Task 3
<p>The sales team wants to run a promotion on upgrades to international travel insurance policies. They only want to send this promotion to customers who have an active, US policy type.</p>
<p>Write a query to provide the customer ID and start date for eligible customers. </p>

## Task 4
<p>After the promotion has been sent, the sales team will need to monitor the number of active policy holders by policy type who purchased an upgrade.  </p>
<p>Write a query that returns the data for the sales team to monitor. Your output should include <code>policy_type</code> and <code>number_active</code> columns.</p>
