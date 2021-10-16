<script>
  import { Router, Link, Route } from "svelte-navigator";
  import StudiosPage from "./pages/StudiosPage.svelte";
  import Home from "./pages/Home.svelte";
</script>

<main>
  <Router>
    <h1>Lampreia Viva</h1>
    <nav>
      <Link to="/">Home</Link>
      <Link to="studios">Studios</Link>
    </nav>
    <div>
      <Route path="/">
        <Home />
      </Route>
      <Route path="/studios">
        <StudiosPage />
      </Route>
    </div>
  </Router>
</main>

<style>
</style>
