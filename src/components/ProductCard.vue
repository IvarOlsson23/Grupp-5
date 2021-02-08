<template>
  <b-container>
    <b-row align-h="center">
      <b-col>
        <!-- product card -->
        <b-card class="overflow-hidden" style="max-width: 540px">
          <img src="../assets/suit.png" alt="suit" />
          <b-card-text>
            <h3>Produkt</h3>
            <p>2900 sek</p>
            <p>Här kan man skiva info om produkter</p>
            <!-- Color dots -->
            <div id="dots">
              <b-icon icon="circle-fill" variant="success"></b-icon>
              <b-icon icon="circle-fill" variant="warning"></b-icon>
              <b-icon icon="circle-fill" variant="danger"></b-icon>
              <b-icon icon="circle-fill" variant="info"></b-icon>
            </div>
            <!-- Add to cart button -->
            <b-button pill variant="primary">Add to Cart</b-button>
          </b-card-text>
        </b-card>
      </b-col>

      <b-col>
        <!-- product card -->
        <b-card class="overflow-hidden" style="max-width: 540px">
          <img src="../assets/suit.png" alt="Suit" />
          <b-card-text>
            <h3>Produkt</h3>
            <p>2900 sek</p>
            <p>Här kan man skiva info om produkter</p>
            <!-- Color dots -->
            <div id="dots">
              <b-icon icon="circle-fill" variant="success"></b-icon>
              <b-icon icon="circle-fill" variant="warning"></b-icon>
            </div>
            <!-- Add to cart button -->
            <b-button pill variant="primary">Add to Cart</b-button>
          </b-card-text>
        </b-card>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  props: {},
};
</script>

<style scoped>
img {
  max-width: 100%;
}
</style>

