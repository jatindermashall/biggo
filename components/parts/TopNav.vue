<template>
  <!--Navbar-->
  <nav
    class="navbar navbar-expand-md navigation-clean-search"
    style="background-color: rgb(34, 34, 34);"
  >
    <div class="container bg-transparent">
      <a class="navbar-brand" :href="host">Biggmind</a>
      <button data-toggle="collapse" class="navbar-toggler bg-transparent" data-target="#navcol-1">
        <span class="sr-only">Toggle navigation</span>
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse bg-transparent navbar-collapse justify-content-end" id="navcol-1">
        <ul class="nav navbar-nav">
          <li class="nav-item" role="presentation">
            <a class="nav-link active" :href="host">Home</a>
          </li>
          <li class="nav-item" role="presentation">
            <a class="nav-link" :href="host + 'profiles'">Profiles</a>
          </li>
          <li class="nav-item" role="presentation">
            <a class="nav-link" :href="host + 'news'">News</a>
          </li>
        </ul>
        <a
          class="btn action-button"
          style="
              background-color: #e0fbfc !important;
              color: #253237 !important;
            "
          role="button"
          href="#"
        >Login</a>
      </div>
    </div>
  </nav>
  <!--Navbar ends here-->
</template>

<script>
export default {
  data() {
    return {
      host: process.env.baseUrl
    };
  }
};
</script>

<style></style>
