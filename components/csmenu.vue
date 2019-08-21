<template>
  <div>
      <nav class="navbar navbar-expand-sm navbar-light bg-light">
          <a class="navbar-brand" href="#">CS MENU</a>
          <button class="navbar-toggler d-lg-none" type="button" data-toggle="collapse" data-target="#collapsibleNavId" aria-controls="collapsibleNavId"
              aria-expanded="false" aria-label="Toggle navigation">
              <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="collapsibleNavId">
              <ul class="navbar-nav mr-auto mt-2 mt-lg-0">
                  <li class="nav-item active">
                      <a class="nav-link" href="/">Home <span class="sr-only">(current)</span></a>
                  </li>
                  <li class="nav-item">
                      <nuxt-link to="/product" class="nav-link">Product</nuxt-link>
                  </li>
                  <li class="nav-item">
                      <nuxt-link to="/showcase" class="nav-link">Show Case</nuxt-link>
                  </li>
                  <li class="nav-item">
                      <nuxt-link to="/about" class="nav-link">About</nuxt-link>
                  </li>
              </ul>
              <form class="form-inline my-2 my-lg-0">
                  <input class="form-control mr-sm-2" type="text" placeholder="Search">
                  <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
              </form>
          </div>
      </nav>
  </div>
</template>

<script>
export default {
    name: 'csmenu'
}
</script>

<style>

</style>