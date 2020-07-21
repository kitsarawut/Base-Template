# Base-Template
Bootstrap 4 Base Template
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Uncle Fruits</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.0/js/bootstrap.min.js"></script>
</head>
<body>

<div class="jumbotron text-center">
  <h1>Uncle Fruits</h1>
    <h3> 
          <a href="{% url 'home-page' %}">หน้าแรก</a>|
          <a href="{% url 'about-page' %}">เกี่ยวกับเรา</a>| 
          <a href="{% url 'contact-page' %}">ติดต่อเรา</a>| 
          <a href="{% url 'allproduct-page' %}">สินค้าทั้งหมด</a>|
          <a href="{% url 'addproduct-page' %}">เพิ่มสินค้า</a>
    </h3> 
</div>


<div class="container">
    {% block content %}
    {% endblock content %}
</div>




</body>
</html>
