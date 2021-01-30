<template>
  <div id="header">
    <ul id=”button”>
      <li><a href=”#”>Sucursales </a></li>
          <li><a href=”#”>Productos y Servicios </a></li>
          <li><a href=”#”>Stock </a></li>
          <li><a href=”#”>Punto de Venta </a></li>
      <li><a href=”#”>Otros </a></li>      
    </ul>   
  </div>
    
    

</template>

<script>
export default {
  name: 'Cabecera',
  data: () => ({
    //
    sucursuales_items: [
        { title: 'Perfiles de Acceso' },
        { title: 'Manejo de Usuarios' },
        { title: 'Manejo de Sucursales' },
      ],
    productosyservicios_items: [
        { title: 'Tipo de Producto o Servicio' },
        { title: 'Ingreso de Productos o Servicios' },
        { title: 'Lista de Precios' },
        { title: 'Diseño de Packs' },
      ],
    stock_items: [
        { title: 'Recepcion' },
        { title: 'Costos' },
        { title: 'Consumo' },
        { title: 'Stock Critico' },
        { title: 'Stock Actual' },
        { title: 'Toma de Inventario' },
      ],
      puntodeventa_items: [
        { title: 'Despacho' },
        { title: 'Devolucion' },
        { title: 'Cierre de Caja' },
        { title: 'Reportes' },
        { title: 'Busqueda de Documentos' },
      ],
      otros_items: [
        { title: 'Monedas' },
        { title: 'Formas de Pago' },
        { title: 'Manejo de Sucursales' },
      ],
  }),
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>		
  #header {
    padding: 0;
    
  }

  #header li {
    display: inline;
  }

  #header li a {
    font-family: Arial;
    font-size: 11px;
    text-decoration: none;
    float: left;
    padding: 10px;
    background-color: #2175bc;
    color: #fff;
  }

  #header li a:hover {
    background-color: #2586d7;
    margin-top: -2;
    padding-bottom: 12px;
  }

</style>