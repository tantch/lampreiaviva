<script>
  import { Router, Link, Route } from "svelte-navigator";
  import HomePage from "./pages/HomePage.svelte";
  import ClientsPage from "./pages/ClientsPage.svelte";
  import EventsPage from "./pages/EventsPage.svelte";
  import AboutPage from "./pages/AboutPage.svelte";
  import ContactsPage from "./pages/ContactsPage.svelte";

  import "App.css";
</script>

<main>
  <Router>
    <div class="header">
      <Link to="/">Estúdio</Link>
      <Link to="/clientes">Clientes</Link>
      <Link to="/eventos">Eventos</Link>
      <Link to="/sobre">Sobre</Link>
      <Link to="/contactos">Contactos</Link>
    </div>
    <div class="home-title">
      <div>Lampreia</div>
      <div>Viva</div>
    </div>
    <div class="title-break" />
    <div>
      <Route path="/">
        <HomePage />
      </Route>
      <Route path="/clientes">
        <ClientsPage />
      </Route>
      <Route path="/eventos">
        <EventsPage />
      </Route>
      <Route path="/sobre">
        <AboutPage />
      </Route>
      <Route path="/contactos">
        <ContactsPage />
      </Route>
    </div>
  </Router>
</main>


<style>
  main {
    display:flex;
    flex-direction: column;
    align-items: center;
  }
  .home-title {
    font-size: 70px;
    font-weight: 100;
    text-align: center;
    margin: 20px;
  }
  .home-title > * {
    margin:0;
  }
  .title-break{
    width: 220px;
    border-bottom: 1px solid black;
  }
</style>
