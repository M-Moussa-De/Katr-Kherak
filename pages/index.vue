<template>
  <div id="app">
    <Nav />

    <!-- Hero section -->
    <section id="hero">
      <b-carousel id="hero-carousel" :interval="10000" controls>
        <b-carousel-slide
          v-for="hero in heros"
          :key="hero.id"
          :caption="`${hero.caption}`"
          :text="`${hero.text}`"
          :img-src="`${hero.src}`"
        ></b-carousel-slide>
      </b-carousel>
    </section>
    <!-- End hero section -->

    <!-- Why we here -->
    <section id="why-we-here">
      <div class="container">
        <h3 class="header">WHY ARE WE HERE?</h3>
        <p class="text mb-0">
          Every day delicious, fresh food goes to waste in supermarkets,
          cafeterias, restaurants, hotels, stores, individual and manufacturers,
          simply because it has not been sold or used on time.
        </p>
        <p class="text mt-0">
          This situation should be over, and that's why we are. Our aim is to
          make usage as most as possible of the extra food and to deliver ot to
          the people in need.
        </p>
        <figure>
          <q
            cite="https://www.wfp.org/stories/5-facts-about-food-waste-and-hunger"
            >Global hunger isn't about a lack of food. Right now, the world
            produces enough food to nourish every child, woman and man on the
            planet.</q
          >
          <figcaption>According to WFP June 2020</figcaption>
        </figure>
      </div>
    </section>
    <!-- End why we here -->

    <!-- Facts -->
    <section id="facts">
      <div class="row">
        <div v-for="fact of facts" :key="fact.id" class="col">
          <img :src="`${fact.icon}`" :alt="`${fact.title}`" />
          <h4>{{ fact.number }}</h4>
          <h5>{{ fact.title }}</h5>
        </div>
      </div>
    </section>
    <!-- End facts -->

    <!-- Donators signup -->
    <section id="donators">
      <div class="container">
        <h3 class="header">Give help to the people in need?</h3>
        <div class="row">
          <!-- Left -->
          <div class="col-12 col-md-6 mb-5">
            <h3>Register your business with surplus food</h3>
            <h4>Be part of the solution</h4>

            <p class="text">
              We are in the middle between your extra food the people in need.
              Our volunteers will make sure to deliver it to those people.
            </p>

            <NuxtLink class="btn" to="/signup_business"
              >Sign up your business</NuxtLink
            >
          </div>

          <!-- Right -->
          <div class="col-12 col-md-6">
            <img src="/images/hero.jpg" alt="Be apart of the solution" />
          </div>
        </div>
      </div>
    </section>
    <!-- End donators signup -->

    <!-- Our partners -->
    <section id="partners">
      <div class="overlay"></div>
      <div class="row">
        <div v-for="partner of partners" :key="partner.id" class="col-md-3">
          <b-img
            class="partner"
            :src="`${partner.src}`"
            :alt="`${partner.name} logo`"
            :title="`${partner.name}`"
          ></b-img>
        </div>
      </div>
    </section>
    <!-- End our partners -->

    <!-- Footer -->
    <Footer />
    <!-- End footer -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      heros: [
        {
          id: 1,
          caption:
            "Nearly a third of all food produced each year is squandered or lost before it can be consumed",
          text: "After UN report, September 2013",
          src: "/images/hero.jpg",
        },
        {
          id: 2,
          caption:
            "Egypt climbs the top of the highest contributing countries to food waste percentages",
          text: "According to a study for BCFN",
          src: "/images/hero2.jpg",
        },
        {
          id: 3,
          caption:
            "In developing countries, 40% of losses occur at post-harvest and processing levels",
          text: "After WFP 2020",
          src: "/images/hero3.jpg",
        },
      ],
      facts: [
        {
          id: 1,
          number: 10245,
          title: "Kilos food delivered",
          icon: "/images/fact1.png",
        },
        {
          id: 2,
          number: 25461,
          title: "Plates of food delivered",
          icon: "/images/fact2.png",
        },
        {
          id: 3,
          number: 3241,
          title: "Recycled waste",
          icon: "/images/fact3.png",
        },
        {
          id: 4,
          number: 41245,
          title: "People served",
          icon: "/images/fact4.png",
        },
        {
          id: 5,
          number: 32154,
          title: "Benefit organizations",
          icon: "/images/fact5.png",
        },
        {
          id: 6,
          number: 18452,
          title: "Help recived",
          icon: "/images/fact6.png",
        },
      ],
      partners: [
        { id: 1, name: "Hardees", src: "/images/partners/hardees.png" },
        { id: 2, name: "Chilis", src: "/images/partners/chilis.png" },
        { id: 3, name: "Unicef", src: "/images/partners/unicef.png" },
        { id: 4, name: "Campisis", src: "/images/partners/campisis.png" },
      ],
    };
  },
};
</script>

<style lang="scss">
// Hero
section#hero {
  #hero-carousel {
    position: relative;
    img {
      min-height: 60rem !important;
      max-height: 60rem !important;
      height: 60rem !important;
      object-fit: cover;
    }
    .carousel-caption {
      background: #1b8989bf;
      color: var(--color-white);
      max-width: 50rem;
      padding: 3rem 2rem;
      text-align: left;

      h3 {
        font-size: 2.2rem;
        font-weight: 400;
        line-height: 1.4;
      }

      p {
        position: absolute;
        left: 2em;
        bottom: 0;
        font-size: 1rem;
      }
    }
  }
}

// Why we here
section#why-we-here {
  figure {
    color: var(--color-dark-navy);
    font-size: 2rem;
    // margin-top: 2rem;

    q {
      margin-bottom: 0;
      font-weight: 700;
    }

    figcaption {
      font-size: 1.2rem;
    }
  }

  .text {
    color: var(--color-dark-navy);
    font-size: 2rem;
  }

  figure {
    color: var(--color-dark-navy);
    font-size: 2rem;
    margin-top: 2rem;

    q {
      margin-bottom: 0;
    }

    figcaption {
      font-size: 1.2rem;
    }
  }
}

// Facts
section#facts {
  background: var(--color-light-navy);

  .col {
    text-align: center;
    margin-bottom: 2rem;
    @media (min-width: 990px) {
      margin-bottom: 0;
    }

    img {
      width: 90px;
    }

    h4 {
      color: var(--color-white);
      font-weight: 700;
      font-size: 2.6rem;
    }

    h5 {
      color: var(--color-white);
    }
  }
}

// Donators signup
section#donators {
  padding-top: 10rem;
  .row {
    display: flex;
    justify-content: space-between;
    align-items: center;

    h3 {
      color: var(--color-dark-navy);
      font-weight: 600;
      font-size: 3rem;
      text-transform: uppercase;
    }

    h4 {
      color: var(--color-2xlight-navy);
      font-weight: 600;
      font-size: 2.5rem;
      margin: 2.8rem 0;
    }

    p {
      color: var(--color-dark-navy);
      font-size: 1.8rem;
      font-weight: 500;
      line-height: 1.5;
    }

    a.btn {
      margin-top: 2rem;
      font-weight: 600;
      text-transform: uppercase;
      text-align: center;
      border: 2px solid var(--color-2xlight-navy);
      border-radius: 10rem;
      color: var(--color-2xlight-navy);
      font-size: 1.5rem;
    }
  }
}

// Partners
section#partners {
  background: var(--color-white);
  margin-top: 5rem;
  padding: 6rem 8rem;
  position: relative;

  img.partner {
    display: block;
    width: 11rem;
    margin: 2rem auto;

    @media (min-width: 990px) {
      margin: 0 auto;
    }
  }
}
</style>
