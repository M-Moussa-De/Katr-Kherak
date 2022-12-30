<template>
  <div>
    <Nav />
    <div id="products">
      <div class="container">
        <div class="row">
          <div
            v-for="product of products"
            :key="product.id"
            class="col-md-4 col-sm-6"
          >
            <div class="card">
              <div class="inner">
                <div class="main-img">
                  <img :src="`${product.src}`" alt="Category" />
                </div>
              </div>
              <div class="card-body text-center">
                <h4 class="card-title">{{ product.title }}</h4>
                <p class="text-muted">{{ product.description }}</p>
                <p class="text-muted">
                  Enough for:
                  <span class="font-weight-bold">{{ product.personsnr }}</span>
                </p>
                <NuxtLink
                  class="btn btn-sm mt-2"
                  :to="`/products/${product.id}`"
                  >View Products</NuxtLink
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <Footer />
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [
        {
          id: 1,
          title: "Tameea and Tahena",
          personsnr: 1,
          description:
            "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Itaque, nulla.",
          src: "/images/products/tameea.png",
        },
        {
          id: 2,
          title: "Fish",
          personsnr: 1,
          description:
            "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Itaque, nulla.",
          src: "/images/products/fish.png",
        },
        {
          id: 3,
          title: "Koshary",
          personsnr: 2,
          description:
            "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Itaque, nulla.",
          src: "/images/products/Koshari.png",
        },
        {
          id: 2,
          title: "Fish",
          personsnr: 1,
          description:
            "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Itaque, nulla.",
          src: "/images/products/fish.png",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
#products {
  margin: 5rem 0;

  .card {
    border: 1px solid #eee;
    padding: 1rem 2rem;
    margin-bottom: 1rem;

    p {
      font-size: 1.4rem;
      text-align: left;
    }

    a.btn {
      background: var(--color-light-navy);
      color: var(--color-white);
      padding: 0.5rem 0.7rem;
    }
  }
}
</style>
