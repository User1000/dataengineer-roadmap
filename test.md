
# aaaa
```mermaid
    graph TD;
    Product[<a  style='text-decoration: none' href='#Product'>Product</a>]
Supplier[<a  style='text-decoration: none' href='#Supplier'>Supplier</a>]
Component[<a  style='text-decoration: none' href='#Component'>Component</a>]
Customer[<a  style='text-decoration: none' href='#Customer'>Customer</a>]
SalesOrderItem[<a  style='text-decoration: none' href='#SalesOrderItem'>SalesOrderItem</a>]


    Customer -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#CustomerOrdersSoi'>CustomerOrdersSoi</a>&nbsp;&nbsp;"| SalesOrderItem
Supplier -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#SupplierDeliversComponent'>SupplierDeliversComponent</a>&nbsp;&nbsp;"| Component
Supplier -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#SupplierDeliversProduct'>SupplierDeliversProduct</a>&nbsp;&nbsp;"| Product
Supplier -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#SupplierSuppliesForProduct'>SupplierSuppliesForProduct</a>&nbsp;&nbsp;"| Product
Supplier -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#SupplierIsQualifiedForComponent'>SupplierIsQualifiedForComponent</a>&nbsp;&nbsp;"| Component
Supplier -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#SupplierIsQualifiedForProduct'>SupplierIsQualifiedForProduct</a>&nbsp;&nbsp;"| Product
SalesOrderItem -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#SoiRefersToProduct'>SoiRefersToProduct</a>&nbsp;&nbsp;"| Product
SalesOrderItem -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#SoiRefersToComponent'>SoiRefersToComponent</a>&nbsp;&nbsp;"| Component
Product -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#ProductUsesComponent'>ProductUsesComponent</a>&nbsp;&nbsp;"| Component
Product -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#ProductUsesProduct'>ProductUsesProduct</a>&nbsp;&nbsp;"| Product
Customer -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#CustomerBuysProduct'>CustomerBuysProduct</a>&nbsp;&nbsp;"| Product
Customer -->|"&nbsp;&nbsp;<a  style='text-decoration: none' href='#CustomerBuysComponent'>CustomerBuysComponent</a>&nbsp;&nbsp;"| Component

```