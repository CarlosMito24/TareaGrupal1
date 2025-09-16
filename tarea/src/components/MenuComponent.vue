<template>
  <div>
    <nav>
      <ul class="menu">
        <li><a href="#">Inicio</a></li>
        <li><a href="#">Perfil</a></li>
        <li><a href="#">Videos</a></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "MenuNav"
}
</script>

<style scoped>
nav {
  background: #1877f2;
  font-size: 18px;
  color: #FFF;
  height: 60px;
  display: flex;
  align-items: center;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.2);
}

.menu {
  list-style: none;
  display: flex;
  justify-content: center;
  gap: 30px;
  width: 100%;
  margin: 0;
  padding: 0;
}

.menu li {
  position: relative;
}

.menu li a {
  color: white;
  text-decoration: none;
  font-weight: bold;
  padding: 8px 12px;
  border-radius: 8px;
  transition: all 0.3s ease;
}

.menu li a:hover {
  background-color: rgba(255, 255, 255, 0.2);
  transform: translateY(-2px);
}
</style>
