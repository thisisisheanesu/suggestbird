<script lang="ts">
  import { Router, Route } from "svelte-routing";
  import Login from "./pages/Login.svelte";

  export let url = ''
</script>

<Router {url}>
    <main>
      <Route path="login" component={Login} />
    </main>
</Router>

