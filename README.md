# mall-credit-management
for an E-commerce store, earn credit and consume credit

Design Consideration:
1. The earn credit rules and consume credit rules, will be managed by other business modules(orders, marketing etc.)
2. The credit management module will simply supply APIs, so other modules can use them to add/reduce credit.

# Database Design
Table: credit_transaction
columns:
| column name  | description |
| ------------ | ----------- |
| id  | detail id  |
| user_id  | user id  |
| channel_id  | earn channel or consume channel id, like order, marketing  |
| event_id  | related event id, for example, order id, comment id, activity id  |
| credit  | earn is positive, consume is negative  |
| created_time  | earn or consume time  |
| expired_time  | credit expire date  |

id -- 
user_id -- user id
channel_id -- earn channel or consume channel id, like order, marketing
event_id -- related event id, for example, order id, comment id, activity id
credit -- earn is positive, consume is negative
created_time -- earn or consume time
expired_time -- credit expire date

# API Design
name 

Business Object Design
