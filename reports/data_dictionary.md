# Lab 1 - Olist E-Commerce Dataset Data Dictionary

## Overview

The Olist Brazilian E-Commerce Dataset consists of multiple related tables representing customers, orders, products, sellers, reviews, payments, and geographical information.

---
# | Table           | Column                        | Data Type | Description                                             | Example Value                      |
| --------------- | ----------------------------- | --------- | ------------------------------------------------------- | ---------------------------------- |
| **customers**   | customer_id                   | String    | Unique customer identifier for each order               | `06b8999e2fba1a1fbc88172c00ba8bc7` |
| customers       | customer_unique_id            | String    | Unique identifier for a customer across multiple orders | `861eff4711a542e4b93843c6dd7febb0` |
| customers       | customer_zip_code_prefix      | Integer   | Customer ZIP code prefix                                | `14409`                            |
| customers       | customer_city                 | String    | Customer's city                                         | `franca`                           |
| customers       | customer_state                | String    | Customer's state abbreviation                           | `SP`                               |
| **orders**      | order_id                      | String    | Unique order identifier                                 | `e481f51cbdc54678b7cc49136f2d6af7` |
| orders          | customer_id                   | String    | Customer who placed the order                           | `9ef432eb6251297304e76186b10a928d` |
| orders          | order_status                  | String    | Current status of the order                             | `delivered`                        |
| orders          | order_purchase_timestamp      | Datetime  | Date and time when the order was placed                 | `2017-10-02 10:56:33`              |
| orders          | order_approved_at             | Datetime  | Date and time when payment was approved                 | `2017-10-02 11:07:15`              |
| orders          | order_delivered_carrier_date  | Datetime  | Date when the order was handed to the carrier           | `2017-10-04 19:55:00`              |
| orders          | order_delivered_customer_date | Datetime  | Date when the customer received the order               | `2017-10-10 21:25:13`              |
| orders          | order_estimated_delivery_date | Datetime  | Estimated delivery date                                 | `2017-10-18 00:00:00`              |
| **order_items** | order_id                      | String    | Order identifier                                        | `00010242fe8c5a6d1ba2dd792cb16214` |
| order_items     | order_item_id                 | Integer   | Item number within the order                            | `1`                                |
| order_items     | product_id                    | String    | Identifier of the purchased product                     | `4244733e06e7ecb4970a6e2683c13e61` |
| order_items     | seller_id                     | String    | Identifier of the seller                                | `48436dade18ac8b2bce089ec2a041202` |
| order_items     | shipping_limit_date           | Datetime  | Shipping deadline for the seller                        | `2017-09-19 09:45:35`              |
| order_items     | price                         | Float     | Price of the product                                    | `58.90`                            |
| order_items     | freight_value                 | Float     | Shipping cost charged for the item                      | `13.29`                            |


