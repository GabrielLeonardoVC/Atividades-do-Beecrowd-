# Atividades-do-Beecrowd-
## Atividades Nível 1
- 2603 - Nível 1
    
    <img width="1920" height="892" alt="Image" src="https://github.com/user-attachments/assets/8fc16bcb-2330-46e7-ab08-d389b99c8d27" />
    
    ```python
    SELECT
        name,
        street
    FROM
        customers
    WHERE
        city = 'Porto Alegre';
    
    ```
    
- 2607 - Nível 1
    
    <img width="1898" height="835" alt="Image" src="https://github.com/user-attachments/assets/f0575834-a668-498b-9e3c-d4a8c3960000" />
    
    ```python
    SELECT DISTINCT
        city
    FROM
        providers
    ORDER BY
        city ASC;
    
    ```
    
- 2608 - Nível 1
    
    <img width="1919" height="839" alt="Image" src="https://github.com/user-attachments/assets/ff80bd98-9ec4-46bd-9c76-dac400e3cc2f" />
    
    ```python
    SELECT
        MAX(price) AS max_price,
        MIN(price) AS min_price
    FROM
        products;
    ```
    
- 2615 - Nível 1
    
    <img width="1920" height="895" alt="Image" src="https://github.com/user-attachments/assets/9a5275d0-13e7-4ddb-a693-c48cb5667f31" />
    
    ```python
    SELECT DISTINCT city
    FROM customers;
    
    ```
    
- 2622 - Nível 1
    
    <img width="1920" height="888" alt="Image" src="https://github.com/user-attachments/assets/e7613e59-30a8-499f-ab3a-7af8f1a69350" />
    
    ```python
    SELECT 
        name
    FROM
        Customers
    Where
    id in(SELECT id_customers FROM legal_person);
    ```
## Atividades Nível 2
- 2604 - Nível 2
    
    <img width="1891" height="831" alt="Image" src="https://github.com/user-attachments/assets/658ddf96-f557-456c-baa3-ba597af58d3d" />
    
    ```python
    SELECT
        id,
        name
    FROM
        products
    WHERE
        price < 10
        OR price > 100;
    ```
    
- 2613 - Nível 2
    
    <img width="1920" height="886" alt="Image" src="https://github.com/user-attachments/assets/38889961-648f-48ac-b07b-aa5abb8490a3" />
    
    ```python
    SELECT
        m.id,
        m.name
    FROM
        movies m
    JOIN
        prices p ON m.id_prices = p.id
    WHERE
        p.value < 2.00;
    ```
## Atividades Nível 3
- 2610 - Nível 3
    
    <img width="1920" height="906" alt="Image" src="https://github.com/user-attachments/assets/d69df490-c5d9-464d-af1d-d74bc3f93753" />
    
    ```python
    SELECT
        ROUND(AVG(price), 2) AS price
    FROM
        products;
    
    ```
    
- 2618 - Nível 3
    
    <img width="1920" height="845" alt="Image" src="https://github.com/user-attachments/assets/91d70174-5592-4025-8a6f-43832a0263db" />
    
    ```python
    SELECT
        p.name AS product_name,
        pr.name AS provider_name,
        c.name AS category_name
    FROM
        products p
    JOIN
        providers pr ON p.id_providers = pr.id
    JOIN
        categories c ON p.id_categories = c.id
    WHERE
        pr.name = 'Sansul SA'
        AND c.name = 'Imported';
    ```
## Atividades Nível 5
- 2614 - Nível 5
    
    <img width="1920" height="902" alt="Image" src="https://github.com/user-attachments/assets/72a0254a-1eb4-4a48-b2fc-8231a0621111" />
    
    ```python
    SELECT
        c.name,
        r.rentals_date
    FROM
        rentals r
    JOIN
        customers c ON r.id_customers = c.id
    WHERE
        r.rentals_date BETWEEN '2016-09-01' AND '2016-09-30';
    ```
