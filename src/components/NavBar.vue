<template>
  <nav class="navbar navbar-expand-sm navbar-dark bg-primary px-3">
      <router-link :to="{name:'Home'}" class="navbar-brand">Blog</router-link>
      <button class="navbar-toggler d-lg-none" type="button" data-toggle="collapse" data-target="#collapsibleNavId" aria-controls="collapsibleNavId"
          aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="collapsibleNavId">
          <ul class="navbar-nav me-auto mt-2 mt-lg-0">
              <li class="nav-item active">
                  <router-link :to="{name:'Dashboard'}" class="nav-link" href="#">Dashboard</router-link>
              </li>
          </ul>
          <ul class="navbar-nav ms-auto mt-2 mt-lg-0">
              <li class="nav-item active">
                  <router-link :to="{name:'Signin'}" class="nav-link" href="#">Signin</router-link>
              </li>
          </ul>
      </div>
  </nav>
</template>

<script>
export default {

}
</script>

<style>

</style>