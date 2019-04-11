<template>
  <div>
    <b-card title="We deal in">
      <b-list-group>
        <b-list-group-item>Dental Materials</b-list-group-item>
        <b-list-group-item>Dental Chair</b-list-group-item>
        <b-list-group-item>Dental Instruments and Accessories</b-list-group-item>
      </b-list-group>
      <b-button variant="primary" href="#">More Info</b-button>
    </b-card>
    <div class="cards">
      <b-card
        title="Dental Lab"
        :img-src="h1"
        img-alt="dentallab"
        img-top
        tag="feature"
        style="max-width: 20rem;"
        class="mb-2"
      >
        <b-card-text>In our Dental Lab, so many things are happening.</b-card-text>
        <b-button href="#" variant="primary">Know more</b-button>
      </b-card>
      <b-card
        title="Dental Store"
        :img-src="h56"
        img-alt="dentalstore"
        img-top
        tag="feature"
        style="max-width: 20rem;"
        class="mb-2"
      >
        <b-card-text>Complete your venture with our state-of-art products</b-card-text>
        <b-button href="#" variant="primary">Know more</b-button>
      </b-card>
    </div>
    <b-card header="Contact us" class="text-center" style="max-width: 40rem;">
      <b-card-text>
        <i class="fas fa-envelope"></i>
        <a href="mailto:dentorder8@gmail.com">dentorder8@gmail.com</a>
        <br>
        <i class="fa fa-phone"></i>
        <a href="tel:+918826355824">+91 8826 355824</a>
        <br>
        <i class="fa fa-phone"></i>
        <a href="tel:+919612465364">+91 9612 465364</a>
        <br>
        <i class="fa fa-phone"></i>
        <a href="tel:+919210069499">+91 9210 069499</a>
      </b-card-text>
    </b-card>
  </div>
</template>
<script>
import h1 from "../assets/1.jpg";
import h56 from "../assets/56.jpg";
export default {
  name: "highlights",
  data() {
    return {
      h1: h1,
      h56: h56
    };
  }
};
</script>
<style>
b-card {
  max-width: 20rem;
}
.cards {
  display: flex;
  justify-content: space-evenly;
}
.text-center {
  margin: 0 auto;
  font-size: 12px;
}
@media only screen and (max-width: 600px) {
  .cards {
    display:block;
  }
}
</style>
