<template>
  <div class="bg-base-200 px-20">
    <div class="navbar">
      <div class="navbar-start">
        <div class="dropdown">
          <div tabindex="0" role="button" class="btn btn-ghost lg:hidden">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h8m-8 6h16" />
            </svg>
          </div>
          <ul tabindex="0" class="menu menu-sm dropdown-content bg-base-100 rounded-box z-1 mt-3 w-52 p-2 shadow">
            <li><a>Item 1</a></li>
            <li>
              <a>Parent</a>
              <ul class="p-2">
                <li><a>Submenu 1</a></li>
                <li><a>Submenu 2</a></li>
              </ul>
            </li>
            <li><a>Item 3</a></li>
          </ul>
        </div>
        <a class="cursor-pointer"><img class="w-20" :src="'img/logo.png'" alt="" /></a>
      </div>
      <div class="navbar-center hidden lg:flex">
        <ul class="menu menu-horizontal gap-8 text-base-100 text-lg px-1">
          <li><a class="rounded-md">Home</a></li>
          <li><a class="rounded-md">Courses</a></li>
          <li><a class="rounded-md">Careers</a></li>
          <li><a class="rounded-md">Blog</a></li>
          <li><a class="rounded-md">About Us</a></li>
        </ul>
      </div>
      <div class="navbar-end gap-4">
        <button class="btn bg-base-100 rounded-3xl px-8">Login</button>
        <button class="btn bg-success rounded-3xl px-8 text-base-100">Sign up</button>
      </div>
    </div>
  </div>
</template>
