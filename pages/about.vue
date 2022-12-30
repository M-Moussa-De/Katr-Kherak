<template>
  <div>
    <Nav />

    <div id="about">
      <div class="container">
        <div class="row">
          <div class="col-md-2">
            <aside>
              <h4>About us</h4>
              <ul>
                <li><a href="#our_work">What we do</a></li>
                <li><a href="#our_mission">Our mission</a></li>
                <li><a href="#our_vision">Our vision</a></li>
                <li><a href="#our_staff">Our staff</a></li>
                <li><a href="#our_partners">Our Partners</a></li>
              </ul>
            </aside>
          </div>

          <div class="col-md-10">
            <h1>What we do</h1>
            <article id="our_work">
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus
                tempore alias, ipsam perferendis laborum, quod beatae cumque
                voluptas libero, perspiciatis vero! Eum cumque similique dolores
                possimus quaerat reiciendis architecto adipisci veritatis
                emmagnam fugit doloribus, id recusandae. Quos sed itaque at
                <strong>2000</strong> voluptates nulla.
              </p>
              <p>
                Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                Quisquam exercitationem blanditiis molestiae aperiam aspernatur
                in rem, adipisci eaque officia cupiditate sapiente cum veritatis
                quaerat perspiciatis ad <strong>1713</strong> sit dolore omnis
                voluptatum laborum repellendus est. Libero?
              </p>

              <h3>Reducing Food waste and fighting hunger</h3>

              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Autem
                dolorum exercitationem nisi in enim qui non culpa, quos
                molestiae, hic magnam vel magni consequatur! Veritatis
                consequuntur, pariatur exercitationem necessitatibus nesciunt
                totam, labore fugit ipsam nisi at, amet vero reiciendis. Illo.
              </p>
              <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Minima
                adipisci ratione hic aspernatur voluptatum tenetur. Unde quod
                libero dolore laboriosam. Placeat laborum unde commodi velit
                quasi minus aperiam provident impedit dolore nesciunt, delectus
                blanditiis ipsam corrupti sequi ex illum! Deleniti!
              </p>
            </article>

            <article id="our_mission">
              <h2>Our Mission</h2>
              <em
                >Provide food, hope and dignity to our neighbors who struggle
                with hunger, and lead the movement to alleviate hunger through
                education, collaboration and advocacy.
              </em>
            </article>

            <article id="our_vision">
              <h2>Our Vision</h2>
              <em
                >Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                Dolorem voluptate odio eum recusandae. Minima in impedit quod
                asperiores?
              </em>
            </article>

            <!-- Our staff -->
            <article id="our_staff">
              <h2 class="staff">Our amazing staff</h2>

              <div class="row">
                <div class="col-md-3">
                  <img src="/images/staff/tarek.png" alt="Dr. Tarek Ali" />
                  <strong class="d-block">Dr. Tarek Ali - Supervision</strong>
                </div>
              </div>

              <div class="row">
                <div class="col-md-4">
                  <img src="/images/staff/mahmoud_abdallah.png" alt="" />
                  <strong class="d-block"
                    >Mahmoud AbdAllah - Business owner</strong
                  >
                </div>
                <div class="col-md-4">
                  <img src="/images/staff/ali.png" alt="" />
                  <strong class="d-block"> Ali Younes- Product manager</strong>
                </div>
                <div class="col-md-4">
                  <img src="/images/staff/mahmoud_hassanein2.png" alt="" />
                  <strong class="d-block"
                    >Mahmoud Hassanein Mahmoud - Full stack</strong
                  >
                </div>
                <div class="col-md-4">
                  <img src="/images/staff/amr.png" alt="" />
                  <strong class="d-block"
                    >Amr Ameen AbdElmoneem - Devops</strong
                  >
                </div>
                <div class="col-md-4">
                  <img src="/images/staff/mazen.png" alt="" />
                  <strong class="d-block"
                    >Mazen AbdAllah Farag - .Net Developer</strong
                  >
                </div>
                <div class="col-md-4">
                  <img src="/images/staff/marwa.png" alt="" />
                  <strong class="d-block"
                    >Marwa Hashem Ahmed - Frontend developer
                  </strong>
                </div>
                <div class="col-md-4">
                  <img src="/images/staff/yasser.png" alt="" />
                  <strong class="d-block"
                    >Yasser Saed Ali AlMagrabe - Database admin</strong
                  >
                </div>
                <div class="col-md-4">
                  <img src="/images/staff/walead.png" alt="" />
                  <strong class="d-block"
                    >Walead Adel Mohamed - Quality control</strong
                  >
                </div>
              </div>
            </article>
          </div>
        </div>
      </div>
    </div>

    <Footer />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
#about {
  margin-bottom: 6rem;
  padding-top: 5rem;

  h1 {
    text-transform: capitalize;
    margin-bottom: 1rem;
    color: var(--color-dark-navy);
  }

  aside {
    h4 {
      color: var(--color-dark-navy);
    }

    ul li {
      margin: 1rem 0;

      a {
        color: var(--color-light-navy);
      }
    }
  }

  article {
    margin: 2rem 0;

    p,
    em {
      font-size: 1.4rem;
    }

    h3 {
      color: var(--color-light-navy);
      text-transform: capitalize;
    }

    h2 {
      font-size: 2.5rem;
    }
  }

  #our_staff {
    .staff {
      margin: 3rem 0 4rem 0;
    }

    div[class^="col-"] {
      margin: 2rem 0;

      img {
        width: 180px;
        height: 180px;
        object-fit: contain;
        display: block;
        margin: 0 auto;
      }

      strong {
        font-size: 1.4rem;
        text-align: center;
      }
    }
  }
}
</style>
