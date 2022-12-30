<template>
  <div id="donate">
    <div class="container mt-5">
      <NuxtLink class="text-muted" to="/"
        ><b-icon icon="arrow-left"></b-icon> Back to home</NuxtLink
      >
      <b-form>
        <h2 class="text-center my-5">Become a volunteer</h2>
        <div class="row">
          <div class="col-md-6">
            <b-form-group label="First name:" label-for="firstname">
              <b-form-input
                id="firstname"
                type="text"
                placeholder="Enter your firstname"
              ></b-form-input>
            </b-form-group>
          </div>

          <div class="col-md-6">
            <b-form-group label="Last name:" label-for="lastname">
              <b-form-input
                id="lastname"
                type="text"
                placeholder="Enter your lastname"
              ></b-form-input>
            </b-form-group>
          </div>

          <div class="col-md-6">
            <b-form-group label="National ID:" label-for="id">
              <b-form-input
                id="id"
                type="text"
                placeholder="Enter your national ID"
              ></b-form-input>
            </b-form-group>
          </div>

          <div class="col-md-6">
            <b-form-group label="Email:" label-for="email">
              <b-form-input
                id="email"
                type="text"
                placeholder="Enter your email"
              ></b-form-input>
            </b-form-group>
          </div>

          <div class="col-md-6">
            <b-form-group label="Address:" label-for="address">
              <b-form-input
                id="address"
                type="tel"
                placeholder="Enter your address"
              ></b-form-input>
            </b-form-group>
          </div>

          <div class="col-md-6">
            <b-form-group label="Phone number:" label-for="phone">
              <b-form-input
                id="phone"
                type="tel"
                placeholder="Enter your phone number"
              ></b-form-input>
            </b-form-group>
          </div>

          <!-- Gender -->
          <div class="col-md-6">
            <label for="">Gender</label>
            <div class="d-flex">
              <div class="form-check">
                <input class="" type="radio" name="gender" id="male" />
                <label class="form-check-label" for="male"> Male </label>
              </div>
              <div class="form-check ml-5">
                <input
                  class=""
                  type="radio"
                  name="gender"
                  id="female"
                  checked
                />
                <label class="form-check-label" for="female"> Femal </label>
              </div>
            </div>
          </div>
          <!--End gender -->

          <div class="col-md-6">
            <label for="extra-notes">Extra notes(Optional):</label>
            <b-form-textarea
              id="extra-notes"
              placeholder="Have notes to write down?"
            ></b-form-textarea>
          </div>

          <div class="col-12 mt-3">
            <div class="form-check">
              <input class="" type="checkbox" value="" id="healthy" />
              <label class="form-check-label" for="healthy">
                I have no health problems, that prevent my work as a volunteer
              </label>
            </div>
          </div>

          <div class="col-12 mt-1">
            <div class="form-check">
              <input class="" type="checkbox" value="" id="age" />
              <label class="form-check-label" for="age">
                I'm over 18 years old
              </label>
            </div>
          </div>

          <div class="col-12 mt-3">
            <b-button type="submit" class="btn btn-sm">Send data</b-button>
          </div>
        </div>
      </b-form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style lang="scss">
#donate {
  button[type="submit"] {
    background: var(--color-dark-navy);
    padding: 0.5rem 2rem;
    text-transform: uppercase;
    border-radius: 10rem;

    &:hover {
      background: lighten($color: #114d4d, $amount: 5);
    }
  }
}
</style>
