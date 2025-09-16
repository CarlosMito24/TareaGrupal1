<template>
    <div class="piedepagina">
        <h2>Miembros del grupo</h2>
        <ol><li>Carlos Alfonso Mito De León</li>
        <li>Melissa Nicole Elena Fuentes</li>
        <li>Kevin Santiago Mate Perez</li>
        <li>Edgardo Israel Tobar Claros</li>
        <li>Josue David Abarca Linares</li></ol>
    </div>
</template>

<script>

</script>

<style>
.piedepagina {
    background-color: #1877f2;
    position: fixed;
    bottom: 0;
    width: 100%;
    padding: 10px;
}
.piedepagina h2 {
  font-size: 20px;
  text-align: center;
  color: #000;
  margin: 20px;
}

.piedepagina ol {
  list-style: none;
  display: flex;
}

.piedepagina li {
  font-size: 15px;
  color: #000;
  background: #ffffff;
  border-radius: 8px;
  padding: 6px 10px;
  margin: 0 auto;
  box-shadow: 0 2px 4px rgba(0,0,0,0.05);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.piedepagina li:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0,0,0,0.08);
}
</style>