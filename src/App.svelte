<script>
// Initialization for ES Users
// import {
//   Datepicker,
//   Input,
//   initTE,
// } from "tw-elements";

// initTE({ Datepicker, Input });

// import { onMount } from "svelte";

// onMount(() => {
//   const myInput = new Input(document.getElementById("myDatepicker"));
//   const options = {
//     format: "dd-mm-yyyy",
//   };
//   const myDatepicker = new Datepicker(
//     document.getElementById("myDatepicker"),
//     options
//   );
// });

</script>

<svelte:head>
  <link href="https://cdn.jsdelivr.net/npm/daisyui@2.51.5/dist/full.css" rel="stylesheet" type="text/css" />
  <link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/npm/tw-elements/dist/css/tw-elements.min.css" />
</svelte:head>
<main>
  <div class="text-sm breadcrumbs">
    <ul>
      <li>
        <a>
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="w-4 h-4 mr-2 stroke-current"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 7v10a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-6l-2-2H5a2 2 0 00-2 2z"></path></svg>
          Home
        </a>
      </li> 
      <li>
        <a>
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="w-4 h-4 mr-2 stroke-current"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 7v10a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-6l-2-2H5a2 2 0 00-2 2z"></path></svg>
          Documents
        </a>
      </li> 
      <li>
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="w-4 h-4 mr-2 stroke-current"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 13h6m-3-3v6m5 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path></svg>
        Add Document
      </li>
    </ul>
  </div>
  <div class="navbar bg-base-100">
    <div class="flex-1">
      <!-- svelte-ignore a11y-missing-attribute -->
      <a class="btn btn-ghost normal-case text-xl">daisyUI</a>
    </div>

    
    <div class="flex-none gap-2">
      <div class="form-control">
        <input type="text" placeholder="Search" class="input input-bordered" />
      </div>
      <div class="dropdown dropdown-end">
        <label tabindex="0" class="btn btn-ghost btn-circle avatar">
          <div class="w-10 rounded-full">
            <img src="/images/stock/photo-1534528741775-53994a69daeb.jpg" />
          </div>
        </label>
        <ul tabindex="0" class="mt-3 p-2 shadow menu menu-compact dropdown-content bg-base-100 rounded-box w-52">
          <li>
            <a class="justify-between">
              Profile
              <span class="badge">New</span>
            </a>
          </li>
          <li><a>Settings</a></li>
          <li><a>Logout</a></li>
        </ul>
      </div>
    </div>
  </div>

  <ul class="steps">
    <li data-content="?" class="step step-neutral">Step 1</li>
    <li data-content="!" class="step step-neutral">Step 2</li>
    <li data-content="✓" class="step step-neutral">Step 3</li>
    <li data-content="✕" class="step step-neutral">Step 4</li>
    <li data-content="★" class="step step-neutral">Step 5</li>
    <li data-content="" class="step step-neutral">Step 6</li>
    <li data-content="●" class="step step-neutral">Step 7</li>
  </ul>


<div class="stats shadow">
  
  <div class="stat">
    <div class="stat-title">Total Page Views</div>
    <div class="stat-value">89,400</div>
    <div class="stat-desc">21% more than last month</div>
  </div>
  
</div>

<div class="divider">OR</div>

<div class="mx-auto w-3/5 overflow-hidden">
  <canvas id="bar-chart"></canvas>
</div>

<div class="grid grid-cols-4 gap-4">
  <div>01</div>
  <div>01</div>
  <div>01</div>
  <div>01</div>
  <div>09</div>
</div>

<div
  class="relative mb-3 xl:w-96"
  data-te-datepicker-init
  data-te-input-wrapper-init>
  <input
    type="text"
    class="peer block min-h-[auto] w-full rounded border-0 bg-transparent px-3 py-[0.32rem] leading-[1.6] outline-none transition-all duration-200 ease-linear focus:placeholder:opacity-100 peer-focus:text-primary data-[te-input-state-active]:placeholder:opacity-100 motion-reduce:transition-none dark:text-neutral-200 dark:placeholder:text-neutral-200 dark:peer-focus:text-primary [&:not([data-te-input-placeholder-active])]:placeholder:opacity-0"
    placeholder="Select a date" />
  <label
    for="floatingInput"
    class="pointer-events-none absolute left-3 top-0 mb-0 max-w-[90%] origin-[0_0] truncate pt-[0.37rem] leading-[1.6] text-neutral-500 transition-all duration-200 ease-out peer-focus:-translate-y-[0.9rem] peer-focus:scale-[0.8] peer-focus:text-primary peer-data-[te-input-state-active]:-translate-y-[0.9rem] peer-data-[te-input-state-active]:scale-[0.8] motion-reduce:transition-none dark:text-neutral-200 dark:peer-focus:text-primary"
    >Select a date</label
  >
</div>

<div class="grid grid-flow-col gap-5 text-center auto-cols-max">
  <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
    <span class="countdown font-mono text-5xl">
      <span style="--value:14;"></span>
    </span>
    days
  </div> 
  <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
    <span class="countdown font-mono text-5xl">
      <span style="--value:10;"></span>
    </span>
    hours
  </div> 
  <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
    <span class="countdown font-mono text-5xl">
      <span style="--value:24;"></span>
    </span>
    min
  </div> 
  <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
    <span class="countdown font-mono text-5xl">
      <span style="--value:23;"></span>
    </span>
    sec
  </div>
</div>



  

  <div class="rating gap-1">
    <input type="radio" name="rating-3" class="mask mask-heart bg-red-400" />
    <input type="radio" name="rating-3" class="mask mask-heart bg-orange-400" checked />
    <input type="radio" name="rating-3" class="mask mask-heart bg-yellow-400" />
    <input type="radio" name="rating-3" class="mask mask-heart bg-lime-400" />
    <input type="radio" name="rating-3" class="mask mask-heart bg-green-400" />
  </div>

  

  

  <div class="indicator">
    <span class="indicator-item badge badge-primary">new</span> 
    <div class="grid w-32 h-32 place-items-center">
      <label class="swap swap-flip text-9xl">
  
        <!-- this hidden checkbox controls the state -->
        <input type="checkbox" />
        
        <div class="swap-on">😈</div>
        <div class="swap-off">😇</div>
      </label>
    </div>
  </div>

  <div class="radial-progress" style="--value:70; --size:12rem; --thickness: 2px;">70%</div>
<div class="radial-progress" style="--value:70; --size:12rem; --thickness: 2rem;">70%</div>

<div class="tooltip" data-tip="hello">
  <button class="btn">Hover me</button>
</div>


  <div class="chat chat-start">
    <div class="chat-image avatar">
      <div class="w-10 rounded-full">
        <img src="/images/stock/photo-1534528741775-53994a69daeb.jpg" />
      </div>
    </div>
    <div class="chat-header">
      Obi-Wan Kenobi
      <time class="text-xs opacity-50">12:45</time>
    </div>
    <div class="chat-bubble">You were the Chosen One!</div>
    <div class="chat-footer opacity-50">
      Delivered
    </div>
  </div>
  <div class="chat chat-end">
    <div class="chat-image avatar">
      <div class="w-10 rounded-full">
        <img src="/images/stock/photo-1534528741775-53994a69daeb.jpg" />
      </div>
    </div>
    <div class="chat-header">
      Anakin
      <time class="text-xs opacity-50">12:46</time>
    </div>
    <div class="chat-bubble">I hate you!</div>
    <div class="chat-footer opacity-50">
      Seen at 12:46
    </div>
  </div>
 

<progress class="progress progress-error w-56" ></progress>

<input type="range" min="0" max="100" value="25" class="range" step="25" />
<div class="w-full flex justify-between text-xs px-2">
  <span>|</span>
  <span>|</span>
  <span>|</span>
  <span>|</span>
  <span>|</span>
</div>
<input type="range" min="0" max="100" value="50" class="range range-sm" /> 
<input type="range" min="0" max="100" value="60" class="range range-md" /> 
<input type="range" min="0" max="100" value="70" class="range range-lg" />

 <!-- The button to open modal -->
<label for="my-modal" class="btn">open modal</label>


<div class="stats shadow">
  
  <div class="stat">
    <div class="stat-figure text-primary">
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-8 h-8 stroke-current"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path></svg>
    </div>
    <div class="stat-title">Total Likes</div>
    <div class="stat-value text-primary">25.6K</div>
    <div class="stat-desc">21% more than last month</div>
  </div>
  
  <div class="stat">
    <div class="stat-figure text-secondary">
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-8 h-8 stroke-current"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
    </div>
    <div class="stat-title">Page Views</div>
    <div class="stat-value text-secondary">2.6M</div>
    <div class="stat-desc">21% more than last month</div>
  </div>
  
  <div class="stat">
    <div class="stat-figure text-secondary">
      <div class="avatar online">
        <div class="w-16 rounded-full">
          <img src="/images/stock/photo-1534528741775-53994a69daeb.jpg" />
        </div>
      </div>
    </div>
    <div class="stat-value">86%</div>
    <div class="stat-title">Tasks done</div>
    <div class="stat-desc text-secondary">31 tasks remaining</div>
  </div>
  
</div>
<!-- Put this part before </body> tag -->
<input type="checkbox" id="my-modal" class="modal-toggle" />
<div class="modal">
  <div class="modal-box">
    <h3 class="font-bold text-lg">Congratulations random Internet user!</h3>
    <p class="py-4">You've been selected for a chance to get one year of subscription to use Wikipedia for free!</p>
    <div class="modal-action">
      <label for="my-modal" class="btn">Yay!</label>
    </div>
  </div>
</div>
  
</main>

<style>
  
</style>
