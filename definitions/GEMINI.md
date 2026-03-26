Use the following naming convention when creating new objects:
* Datasets: [business_domain]_[use_case] (e.g., ecommerce_sales)

* Tables:
    - Raw/External: raw_[source_name]
    - Staging: stg_[business_entity]
    - Dimension: dim_[dimension_name]
    - Fact: fct_[fact_name]

* Dataform Folders:
    - Sources
    - Staging
    - Marts
    - DataProducts

* Views: vw_[view_name]

* Columns: snake_case (e.g., order_id, customer_name)

Always use ${ref()} to ensure dependency between nodes in dataform. ex: ${ref("referenced_sqlx_file")}
