<template>
  <header class="header m-0">
    <b-navbar toggleable="lg" type="light" variant="light">
      <NuxtLink to="/">
        <b-img
          class="logo"
          src="/images/logo.png"
          fluid
          alt="Website logo"
        ></b-img>
      </NuxtLink>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item>
            <NuxtLink class="find-food" aria-current="page" to="/products">
              <b-icon icon="pin-map"></b-icon> Find Food
            </NuxtLink>
          </b-nav-item>

          <b-nav-item>
            <NuxtLink class="donate" aria-current="page" to="/donate">
              <b-icon icon="heart"></b-icon> Donate
            </NuxtLink>
          </b-nav-item>

          <b-nav-item>
            <NuxtLink class="volunteer" aria-current="page" to="/volunteer">
              <b-icon icon="bicycle"></b-icon> Become Volunteer
            </NuxtLink>
          </b-nav-item>

          <b-nav-item>
            <NuxtLink class="about" aria-current="page" to="/about"
              >About us</NuxtLink
            >
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </header>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.header {
  .logo {
    height: 7rem;
  }

  #nav-collapse {
    @media (max-width: 990px) {
      margin-top: 1.5rem;
    }
    ul.navbar-nav {
      li.nav-item {
        margin: 0.5rem 0 0.5rem 1rem;
        @media (max-width: 990px) {
          padding: 0.3rem 1rem;
        }
        &:hover {
          @media (max-width: 990px) {
            background: var(--color-lightgray);
          }
        }

        a {
          text-transform: uppercase;
          font-weight: 600;
          transition: all 0.3s ease;
          color: var(--color-text) !important;

          &.find-food {
            @media (min-width: 990px) {
              border-radius: 100px;
              color: var(--color-white) !important;
              background: var(--color-orange);
              padding: 0.8rem 1.5rem;
            }
          }

          &.donate {
            @media (min-width: 990px) {
              border-radius: 100px;
              color: var(--color-white) !important;
              background: var(--color-green);
              padding: 0.8rem 1.5rem;
            }
          }

          &.volunteer {
            color: var(--color-text) !important;
            @media (min-width: 990px) {
              color: var(--color-white) !important;
              background: var(--color-dark-navy);
              border-radius: 100px;
              padding: 0.8rem 1.5rem;
            }
          }
        }
      }
    }
  }
}
</style>
