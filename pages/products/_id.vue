<template>
  <div>
    <Nav />
    <div id="product">
      <div class="container">
        <div class="row">
          <div class="col-md-4">
            <img src="/images/products/fish.png" alt="Category" />
          </div>
          <div class="col-md-7 ml-md-5">
            <div class="product_details">
              <h3 class="text-uppercase mb-3">Product title</h3>

              <div>
                <h6>Description:</h6>
                <span
                  >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ex
                  rem culpa quae natus eveniet? Molestiae voluptas
                  exercitationem consectetur quam maxime totam.</span
                >
              </div>

              <div>
                <h6 class="mt-3">Ingredients:</h6>
                <ul>
                  <li><span> (15 ounce) container ricotta cheese</span></li>
                  <li>
                    <span>
                      (8 ounce) package shredded mozzarella cheese,
                      divided</span
                    >
                  </li>
                  <li><span> (3 ounce) package Parmesan cheese</span></li>
                  <li><span> egg</span></li>
                  <li><span>2 teaspoons Italian seasoning</span></li>
                  <li><span> pound sausage</span></li>
                  <li><span>½ (26 ounce) jar marinara sauce</span></li>
                  <li><span>6 flatbreads</span></li>
                </ul>
              </div>

              <div>
                <h6 class="mt-3">Extra notes:</h6>
                <span>gluten free</span>
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
    return {};
  },
};
</script>

<style lang="scss" scoped>
#product {
  margin: 8rem 0 0 0;
  min-height: 48vh;

  .product_details {
    display: flex;
    flex-direction: column;
    justify-content: center;
    color: rgba(0 0 0 /0.6);
    height: 100%;
    font-size: 1.6rem;
    @media (max-width: 768px) {
      margin-top: 1rem;

      li {
        color: coral;

        span {
          color: rgba(0 0 0 /0.6);
        }
      }
    }
  }
}
</style>
