![Texto alternativo](ruta-de-la-imagen.jpg)
![Logo del sitio](images/logoEjemplo.jpg)
![Gráfico SVG](images/graph.svg)
<canvas id="myChart" width="400" height="400"></canvas>

<script>
  var ctx = document.getElementById('myChart').getContext('2d');
  var myChart = new Chart(ctx, {
    type: 'bar',
    data: {
      labels: ['Rojo', 'Azul', 'Verde', 'Amarillo'],
      datasets: [{
        label: 'Cantidad de votos',
        data: [12, 19, 3, 5],
        backgroundColor: ['rgba(255, 99, 132, 0.2)', 'rgba(54, 162, 235, 0.2)', 'rgba(75, 192, 192, 0.2)', 'rgba(153, 102, 255, 0.2)'],
        borderColor: ['rgba(255, 99, 132, 1)', 'rgba(54, 162, 235, 1)', 'rgba(75, 192, 192, 1)', 'rgba(153, 102, 255, 1)'],
        borderWidth: 1
      }]
    },
    options: {
      scales: {
        y: { beginAtZero: true }
      }
    }
  });
</script>
