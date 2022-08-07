<script lang="ts">
  import { Router, Route } from "svelte-routing";
  import Login from "./pages/Login.svelte";
  import SignUp from "./pages/SignUp.svelte";

  export let url = ''
</script>

<Router {url}>
    <main>
      <Route path="login" component={Login} />
      <Route path="signup" component={SignUp} /> 
    </main>
</Router>

