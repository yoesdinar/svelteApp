<script>
  import Navbar from "./layout/Navbar.svelte";
  import "../node_modules/materialize-css/dist/css/materialize.min.css";

  import { Router, Link, Route } from "svelte-routing";
  import Home from './pages/Home.svelte';
  import About from './pages/About.svelte'; 
</script>

<style>

</style>

<Router>
  <Navbar />
  <div class="container">
    <Route path="/" component={Home} />
    <Route path="about" component={About} />
  </div>
</Router>
