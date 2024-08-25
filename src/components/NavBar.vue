<script setup></script>

<template>
  <nav class="nav-bar">
    <ul>
      <div class="nav-left">
        <li><a href="#">Home</a></li>
        <li><a href="#">Our Story</a></li>
      </div>
      <div class="hamburger-menu">
        <span class="material-symbols-outlined"></span>
      </div>
      <div class="logo-container">
        <h1 class="logo">con leche.</h1>
        <h2 class="logo-text">coffee house</h2>
      </div>
      <div class="nav-right">
        <li><a href="#">Contact</a></li>
        <li>
          <button class="sign-up-btn"><a href="#">Join Rewards</a></button>
        </li>
      </div>
    </ul>
  </nav>
</template>

<style scoped>
a:link {
  text-decoration: none;
  color: #f6f5eb;
  font-size: 1rem;
  font-weight: 600;
  letter-spacing: 2px;
}
a:visited {
  color: #f6f5eb;
  text-decoration: none;
}
a:hover {
  text-decoration: none;
}
a:active {
  text-decoration: none;
}
.nav-bar li a,
.nav-bar button {
  visibility: hidden;
}

.nav-bar ul {
  width: 100%;
  position: absolute;
  top: 12%;
  transform: translateX(-50%);
  left: 50%;
  display: flex;
  justify-content: space-evenly;
  list-style-type: none;
}

.nav-left,
.nav-right {
  width: 20%;
  display: flex;
  align-items: center;
  justify-content: space-around;
  gap: 40px;
}

.hamburger-menu {
  position: absolute;
  left: 30px;
  top: 30px;
}

.logo-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 8px;
}

.logo {
  color: #f6f5eb;
  font-size: 3rem;
  font-weight: 800;
}

.logo-text {
  color: #f6f5eb;
  text-transform: uppercase;
  margin-top: -12px;
  font-size: 0.6rem;
}

.material-symbols-outlined {
  font-variation-settings: "FILL" 0, "wght" 400, "GRAD" 0, "opsz" 24;
}

@media screen and (min-width: 768px) {
  .logo {
    font-size: 4.5rem;
  }
  .logo-text {
    font-size: 0.8rem;
  }

  .hamburger-menu {
    margin-top: 10px;
  }

  .header-info {
    font-size: 1rem;
  }
}
@media screen and (min-width: 1100px) {
  .hamburger-menu {
    visibility: hidden;
  }
  .nav-bar li a,
  .nav-bar button {
    visibility: visible;
  }
  .sign-up-btn {
    border-radius: 6px;
    border-style: none;
    padding: 10px 15px;
    background-color: rgb(246, 211, 108);
    font-family: "Piazzolla", serif;
    font-weight: 700;
    white-space: nowrap;
  }
  .sign-up-btn a {
    color: #0e2a54;
  }
  .sign-up-btn:hover {
    cursor: pointer;
    background-color: rgb(246, 211, 108, 0.75);
  }
}
</style>
