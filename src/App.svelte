<script lang="ts">
  import { Link, Route, Router } from "svelte-navigator";
  import Inicio from "./pages/inicio.svelte";
  import Politica from "./pages/politica.svelte";
</script>

<Router>
  <nav>
    <Link to="/">Inicio</Link>
    <Link to="politica-privacidad">Politica de privacidad</Link>
  </nav>
  <main>
    <Route path="/">
      <Inicio />
    </Route>
    <Route path="politica-privacidad">
      <Politica />
    </Route>
  </main>
</Router>
