# Analisis-E-commerce

Resumen:

Utilizado el dataset público de pedidos del comercio electrónico brasileño Olist. Se procede a analizar esta información con el fin de encontrar insights que puedan ser transformados en oportunidades de mejora para el negocio.

Todo el proceso de ETL se hace de la siguiente forma. Como primer paso se crea una base de datos utilizado el manejador de PostgreSQL. Después se realizan diferentes querys usando SQL, para transformar, limpiar y mostrar solo la información de interés. A continuación, estos datos más limpias son llevados a Power BI, donde se crea el modelo de los datos, se hacen más transformaciones y limpieza de estos. Cuando todo está listo, se crean los dashasbors para poder analizar la información. 

Link del proyecto: https://sites.google.com/view/julianbarragan/an%C3%A1lisis-del-e-commerce-brasile%C3%B1o-olist?authuser=0

Dataset:

El conjunto de datos está disponible en Kaggle, y está compuesto por nueve archivos con información sobre:

Clientes: Se indican datos del cliente como id e ubicación.
Vendedores: Se indican datos del vendedor como id e ubicación.
Geolocalización: Se usa el zip code, latitud, longitud para tener un posicionamiento exacto de cuidades y estados.
Pedidos: Se da un id a los pedidos junto a las diferentes fechas según el estado de la orden.
Categoría de los productos: Contiene el nombre de las categorías en inglés y portugués.
Review de los pedidos: Se tienen reviews de los diferentes productos.
Descripción del producto: Se dan detalles del tamaño y peso de los productos por categoría.
Métodos de pago: Se describen los diferentes métodos de pago y numero de cuotas.

Pago de los pedidos: Se describe el número de artículos por compra, el cliente id, vendedor id, orden id y el valor total a pagar.
Se cuenta con registros desde octubre del 2016 hasta agosto del 2018, con más de 100.000 ordenes de pedidos diferentes. Estos son datos comerciales reales, por lo tanto para la protección de identidades se han anonimizado, los clientes, vendedores y socios.

# Distribución archivos. 
--------

    ├── Clean data
    │   ├── dim_custumer.csv           <- Datos extraídos de la base de datos de los clientes.
    │   ├── Fact_order_sales.csv       <- Datos extraídos de la base de datos de las ventas por internet.
    │   ├── dim_product.csv            <- Datos extraídos de la base de datos de los productos.
    │   ├── dim_review.csv             <- Datos extraídos de la base de datos de las reviews.
    │   ├── dim_geolocation.csv        <- Datos extraídos de la base de datos de la geolocalizacion.
    │   └── dim_seller.csv             <- Datos extraídos de la base de datos de los clientes..
    │
    ├── SQL Querys
    │   ├── SQLcutomer.sql             <- Query usado para extraer los datos de los clientes.
    │   ├── SQLfact_sales.sql          <- Query usado para extraer los datos de las ventas por internet.
    │   ├── SQLgeolocation.sql         <- Query usado para extraer los datos de la geolocalizacion.
    │   ├── SQLorders.sql              <- Query usado para extraer los datos de las ordes.
    │   ├── SQLproducts.sql            <- Query usado para extraer los datos de los productoss.
    │   └── SQLseller.sql              <- Query usado para extraer los datos de los vendedores.
    │
    ├── Raw data                       <- Archivos extraidos de Kaggle.
    │
    ├── README.md                      <- Toda la información sobre el proyecto.
    │
    ├── proyecto e_commerce.pbix       <- Archivo de POWER BI con los modelos y dashboards creados. 
    │
    └── proyecto e_commerce.pdf        <- Archivo PDF con los 3 dashboards creados.

  --------
