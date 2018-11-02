<template>
  <div id="app">
    <div id="top"></div>

       <!-- icon-nav-wrapper -->
    <div id="icon-nav-wrapper" class="side-nav-inverse">
      
      <!-- side navigation -->
        <a href="#menu-toggle" id="menu-toggle"><i class="fa fa-bars"></i></a>
        <div id="icon-nav-sidebar-wrapper" class="nav-inverse">
            <ul id="nav-scroll" class="sidebar-nav sidebar-nav-inverse">
                <li class="sidebar-brand">
                    <a href="#top" class="smooth-scroll"><img src="images/icon-nav-logo.png" alt=""></a>
                </li>
                <li>
                    <a class="menu-item smooth-scroll nav-link active" href="#top"><i class="md-icon dp24">home</i></a>
                </li>
                <li>
                    <a class="menu-item smooth-scroll nav-link" href="#about"><i class="md-icon dp24">person</i></a>
                </li>
                <li>
                    <a class="menu-item smooth-scroll nav-link" href="#education"><i class="md-icon dp24">school</i></a>
                </li>
                <li>
                    <a class="menu-item smooth-scroll nav-link" href="#experience"><i class="md-icon dp24">work</i></a>
                </li>
                <li>
                    <a class="menu-item smooth-scroll nav-link" href="#work"><i class="md-icon dp24">apps</i></a>
                </li>
                <li>
                    <a class="menu-item smooth-scroll nav-link" href="#contact"><i class="md-icon dp24">email</i></a>
                </li>
            </ul>
        </div>
      <!-- / side navigation -->

    </div>

    <router-view/>

    <footer class="dark bg-inverse">
      <div class="container-fluid text-center">
        <div class="row">
          <div class="col-lg-8 footer-left-area">
            <p>Copyright © 2017. BASIX by <a href="http://kingstudio.ro" target="_blank">KingStudio</a>. All Rights Reserved.</p>
          </div>
          <div class="col-lg-4 social-icons footer-right-area">
            <a href="#x"><i class="fa fa-facebook"></i></a>
            <a href="#x"><i class="fa fa-twitter"></i></a>
            <a href="#x"><i class="fa fa-instagram"></i></a>
            <a href="#x"><i class="fa fa-dribbble"></i></a>
          </div><!-- / social-icons -->
        </div><!-- / row -->
      </div><!-- / container-fluid -->
  </footer>

  </div>
</template>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
