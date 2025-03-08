# Infer-Data-Models-Fix-Quality


+-----------------+          +-----------------+          +-----------------+
|    Product      |          |  Transaction    |          |  Average Costs  |
+-----------------+          +-----------------+          +-----------------+
| Product_ID (PK) |<-------->| Transaction_ID  |<-------->| Product_ID (FK) |
| Name            |          | Product_ID (FK) |          | Date_ID (FK)    |
| Category        |          | Location_ID (FK)|          | Avg_Std_Cost    |
+-----------------+          | Date_ID (FK)    |          | Avg_Landed_Cost |
                             | Quantity        |          +-----------------+
                             | Price           |
                             +-----------------+
                                    |
                                    |
                                    v
+-----------------+          +-----------------+
|    Location     |          |      Date       |
+-----------------+          +-----------------+
| Location_ID (PK)|          | Date_ID (PK)    |
| Name            |          | Date            |
| Address         |          +-----------------+
+-----------------+
