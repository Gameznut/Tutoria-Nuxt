<template>
  <nav
    class="
      flex
      justify-end
      navbar navbar-expand-lg navbar-dark
      bg-blue-400
      py-4
      px-2
      w-full
      bg-dark
      padding
    "
  >
    <NuxtLink class="navbar-brand" to="/">Firengii</NuxtLink>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse ml-auto" id="navbarSupportedContent">
      <ul class="navbar-nav ml-auto flex gap-4">
        <li class="nav-item active">
          <NuxtLink to="/products" class="nav-link"
            >Products <span class="sr-only">(current)</span></NuxtLink
          >
        </li>
        <li class="nav-item active">
          <NuxtLink to="/my-items" class="nav-link"
            >My Items <span class="sr-only">(current)</span></NuxtLink
          >
        </li>
        <li class="nav-item active">
          <NuxtLink to="/calendar" class="nav-link"
            >Calendar <span class="sr-only">(current)</span></NuxtLink
          >
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style></style>
