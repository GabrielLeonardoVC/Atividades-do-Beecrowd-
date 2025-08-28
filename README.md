# Atividades-do-Beecrowd-
- 2603 - Nível 1
    
    ![image.png](attachment:0d372977-8d9f-49a4-8da3-4b4f1af0cc21:image.png)
    
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
    
    ![image.png](attachment:86edfb66-5e0b-4dfe-b914-d8393fd18128:image.png)
    
    ```python
    SELECT DISTINCT
        city
    FROM
        providers
    ORDER BY
        city ASC;
    
    ```
    
- 2608 - Nível 1
    
    ![image.png](attachment:a26ca60f-8230-4586-8c6e-4c8bf3ce8ace:image.png)
    
    ```python
    SELECT
        MAX(price) AS max_price,
        MIN(price) AS min_price
    FROM
        products;
    ```
    
- 2615 - Nível 1
    
    ![image.png](attachment:880e1a88-4ed8-4209-9a16-8ba26a26176e:image.png)
    
    ```python
    SELECT DISTINCT city
    FROM customers;
    
    ```
    
- 2622 - Nível 1
    
    ![image.png](attachment:566f9346-252b-49a3-a942-9f00edb56c3e:image.png)
    
    ```python
    SELECT 
        name
    FROM
        Customers
    Where
    id in(SELECT id_customers FROM legal_person);
    ```
    
- 2604 - Nível 2
    
    ![image.png](attachment:13a4bbbb-d91e-46f2-9065-4de9e0df8d5a:image.png)
    
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
    
    ![image.png](attachment:7274a778-bc35-4f0d-80cd-cae6922f4465:image.png)
    
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
    
- 2610 - Nível 3
    
    ![image.png](attachment:d6313fe1-641c-408e-972a-2ee697878700:image.png)
    
    ```python
    SELECT
        ROUND(AVG(price), 2) AS price
    FROM
        products;
    
    ```
    
- 2618 - Nível 3
    
    ![image.png](attachment:de385b08-a65c-48af-bab1-86b7771be10f:image.png)
    
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
    
- 2614 - Nível 5
    
    ![image.png](attachment:35c7aa66-69ae-4ac7-bab4-2ee90cd0baae:image.png)
    
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
