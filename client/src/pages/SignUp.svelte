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
      <form class="flex flex-col h-full p-8 lg:p-10 md:w-1/2 sm:w-full justify-center items-center">
        <img class="h-24 mb-3" src="suggest-bird.png" alt="Suggest Bird logo">
        <h1 class="mb-4 text-3xl font-bold">Welcome</h1>
        <Input type="text" name="fname" placeholder="First Name" />
        <Input type="text" name="lname" placeholder="Last Name" />
        <Input type="email" name="email" />
        <Input type="password" name="password" autocomplete="new-password" /> 
        <div class="flex w-full flex-row mb-4 justify-between">
          <div class="flex flex-row">
            <Input type="checkbox" name="remember-me" className="mr-1 bg-primary-700 rounded-md" />
            <p class="text-gray-500 text-xs">Remember Me</p>
          </div>
        </div>
        <Button text="Sign Up" />
        <Button text="Sign up with Google" isThirdParty />
        <p class="mt-5 text-md">
          Already have an account?
          <a 
            href="/login"
            class="text-primary-700 hover:text-primary-500">
            Login
          </a>
        </p>
      </form>
    </div>  
  </div>
  
  