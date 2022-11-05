Show Product Stock Status
 Exibe o status de estoque nos modulos e categoria na loja.
 ## A label deve responder como abaixo
 0 = Label Danger
 5 ou menos = Label Warning
 6 ou mais = Label Sucesso
 
```php
<p>{{ text_stock }} 
<span class="label 
{% if (product.quantity <= 0) %}label-danger
{% elseif (product.quantity <= 5) %}label-warning
{% else %}label-success{% endif %}">
{{ product.stock }}</span>
</p>
´´´
![stock_status1](https://user-images.githubusercontent.com/8571832/200137804-34d22eb7-7267-45b8-a31b-77304e7d4a72.jpg)
