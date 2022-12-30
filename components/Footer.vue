<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col-md-3">
          <NuxtLink to="/">
            <b-img
              class="logo"
              src="/images/logo.png"
              alt="Company logo"
            ></b-img>
          </NuxtLink>
          <p class="copyrights">&copy; 2022 Kataar Kherak</p>
        </div>
        <div class="col-md-3 mt-5">
          <h5>Links</h5>
          <ul class="list-unstyled">
            <li><NuxtLink to="/" class="text-muted">Home</NuxtLink></li>
            <li><NuxtLink to="/about" class="text-muted">About</NuxtLink></li>
            <li>
              <NuxtLink to="/signup_business" class="text-muted"
                >Business signup</NuxtLink
              >
            </li>
          </ul>
        </div>
        <div class="col-md-3 mt-5">
          <h5>Contact</h5>
          <ul class="list-unstyled d-flex">
            <li>
              <NuxtLink to="/" class="text-muted">
                <b-icon icon="facebook"></b-icon>
              </NuxtLink>
            </li>
            <li class="mx-4">
              <NuxtLink to="/" class="text-muted">
                <b-icon icon="twitter"></b-icon>
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/" class="text-muted">
                <b-icon icon="instagram"></b-icon>
              </NuxtLink>
            </li>
            <li class="mx-4">
              <NuxtLink to="/" class="text-muted">
                <b-icon icon="google"></b-icon>
              </NuxtLink>
            </li>
          </ul>
        </div>
        <div class="col-md-3 mt-5">
          <h5>Legal</h5>
          <ul class="list-unstyled">
            <li>
              <NuxtLink to="/" class="text-muted">Terms of Service</NuxtLink>
            </li>
            <li>
              <NuxtLink to="/" class="text-muted">Privacy Policy</NuxtLink>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  background: var(--color-lightgray);
  padding: 4rem;
  @media (min-width: 990px) {
    padding: 8rem;
  }

  img.logo {
    width: 9em;
  }

  p.copyrights {
    margin-top: 2em;
    font-size: 1.1rem;
  }
}
</style>
