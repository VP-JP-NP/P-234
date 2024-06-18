select customers.last_name, customers.phone, company_products.name, suppliers.contact_name
from customers join company_orders
on 
customers.id = company_orders.customer_id
join 
suppliers
on company_products.supplier_id = suppliers.id
