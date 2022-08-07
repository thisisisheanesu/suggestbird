<script lang="ts">
  import { Button, Input } from "@components/index";
  import { LottiePlayer } from '@lottiefiles/svelte-lottie-player';
</script>
  
<div class="flex flex-col h-screen w-screen justify-center content-center items-center"> 
  <div class="flex flex-row shadow-lg rounded h-5/6 w-3/4 justify-center items-center">
    <div class="justify-center items-center bg-primary-700 h-full lg:flex hidden lg:w-1/2 rounded-bl-md rounded-tl-md">
      <LottiePlayer
        src="animations/5-star.json"
        autoplay="{true}"
        loop="{true}"
        renderer="svg"
        background="transparent"
        height="{350}"
        width="{300}"
      />  
    </div>
    <form class="flex flex-col p-8 lg:p-12 md:w-1/2 sm:w-full justify-center items-center">
      <img class="h-24 mb-5" src="suggest-bird.png" alt="Suggest Bird logo">
      <h1 class="mb-8 text-3xl font-bold">Welcome Back</h1>
      <Input type="email" name="email" />
      <Input type="password" name="password" autocomplete="current-password" /> 
      <div class="flex w-full flex-row mb-10 justify-between">
        <div class="flex flex-row">
          <Input type="checkbox" name="remember-me" className="mr-1 bg-primary-700 rounded-md" />
          <p class="text-gray-500 text-xs">Remember Me</p>
        </div>
        <a 
          class="text-primary-700 text-xs"
          href="/forgot">
          Forgot password?
        </a>
      </div>
      <Button text="Login" />
      <Button text="Login with Google" isThirdParty />
      <p class="mt-5 text-md">
        Don't have an account?
        <a 
          href="/signup"
          class="text-primary-700 hover:text-primary-500">
          Sign Up
        </a>
      </p>
    </form>
  </div>  
</div>

