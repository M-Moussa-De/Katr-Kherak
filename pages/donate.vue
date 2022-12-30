<template>
  <div id="donate">
    <div class="container mt-5">
      <NuxtLink class="text-muted" to="/"
        ><b-icon icon="arrow-left"></b-icon> Back to home</NuxtLink
      >
      <b-form>
        <h2 class="text-center my-5">Donate a Meal/Dish</h2>
        <div class="row">
          <div class="col-md-6">
            <b-form-group label="Dish title:" label-for="dish-title">
              <b-form-input
                id="dish-title"
                type="text"
                placeholder="Enter your dish name"
              ></b-form-input>
            </b-form-group>
          </div>

          <div class="col-md-6">
            <b-form-group
              label="Dish ingredients:"
              label-for="dish-ingredients"
            >
              <b-form-input
                id="dish-ingredients"
                type="text"
                placeholder="Enter your dish ingredients"
              ></b-form-input>
            </b-form-group>
          </div>

          <div class="col-md-6">
            <b-form-group
              label="Enough for (Persons nr):"
              label-for="enough-for"
            >
              <b-form-input
                id="enough-for"
                type="number"
                min="1"
                value="1"
              ></b-form-input>
            </b-form-group>
          </div>

          <div class="col-md-6">
            <b-form-group label="Dish fotos:" label-for="dish-fotos">
              <b-form-file
                placeholder="Attach fotos for your dish"
                multiple
                id="dish-fotos"
              ></b-form-file>
            </b-form-group>
          </div>

          <div class="col-md-6">
            <b-form-group label="Dish prepared date:" label-for="dish-date">
              <b-form-input id="dish-date" type="date"></b-form-input>
            </b-form-group>
          </div>

          <div class="col-md-6">
            <label for="dish-description">Dish description:</label>
            <b-form-textarea
              id="dish-description"
              placeholder="Describe your dish..."
            ></b-form-textarea>
          </div>

          <div class="col-md-6">
            <label for="extra-notes">Extra notes(Optional):</label>
            <b-form-textarea
              id="extra-notes"
              placeholder="Have notes to write down?"
            ></b-form-textarea>
          </div>

          <div class="col-12 my-3">
            <b-form-checkbox-group
              id="checkboxes-4"
              :aria-describedby="ariaDescribedby"
            >
              <b-form-checkbox value="dash-controlled"
                >The meal was controlled and it's eatable</b-form-checkbox
              >
            </b-form-checkbox-group>
          </div>

          <div class="col-12">
            <b-button type="submit" class="btn btn-sm">Share</b-button>
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
    background: var(--color-green);
    padding: 0.5rem 2rem;
    text-transform: uppercase;
    border-radius: 10rem;

    &:hover {
      background: lighten($color: #a8c257, $amount: 5);
    }
  }
}
</style>
