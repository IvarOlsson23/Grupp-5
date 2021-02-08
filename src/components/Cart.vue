<template>
  <b-container>
    <b-row>
      <b-col>
        <h2>Betalningssätt</h2>
        <b-form @submit.prevent="onSubmitCardDetails">
          <b-form-group
            id="paymentMethod-group"
            label="Betalningsmetod"
            label-for="paymentMethod"
          >
            <b-form-select
              id="payMethod"
              required
              :options="payMethodOptions"
              v-model="receiver.payMethod"
            ></b-form-select>
          </b-form-group>
          <div v-if="receiver.payMethod == 'Visa'">
            <b-form-group
              id="cardNumber-group"
              label="Kortnummer"
              label-for="cardNumber"
            >
              <b-form-input
                id="cardNumber"
                placeholder="0300 XXXX XXXX XXX"
                v-model="receiver.cardNumber"
                required
              ></b-form-input>
            </b-form-group>

            <b-form-group
              id="cardNumberName-group"
              label="Kortinnehavare"
              label-for="cardNumberName"
            >
              <b-form-input
                id="cardNumberName"
                required
                v-model="receiver.cardNumberName"
                placeholder="Jonathan Luxman"
              ></b-form-input>
            </b-form-group>
          </div>
          <div v-else-if="receiver.payMethod == 'Paypal'">
            <b-form-group
              id="paypal-group"
              label="Paypal Konto"
              label-for="paypal"
            >
              <b-form-input
                type="email"
                required
                id="paypal"
                placeholder="Jonathan@paypal.com"
                v-model="receiver.paypalEmail"
              ></b-form-input>
            </b-form-group>
          </div>
          <div v-else-if="receiver.payMethod == 'Bitcoin'">
            <b-form-group
              id="bitcoin-group"
              label="Bitcoin Adress"
              label-for="bitcoinAdress"
            >
              <b-form-input
                required
                id="bitcoinAdress"
                v-model="receiver.bitcoinAdress"
                placeholder="bc1qxy2kgdygjrsqtzq2n0yrf2493p83kkfjhx0wlh"
              ></b-form-input>
            </b-form-group>
          </div>
          <div v-else-if="receiver.payMethod == 'Faktura'">
            <p>Fakturan skickas till din adress</p>
          </div>
        </b-form>
      </b-col>
      <b-col>
        <h2>Kontakt uppgifter</h2>
        <b-form @submit.prevent="Onsubmit">
          <b-form-group id="surname-group" label-for="surname" label="Förnamn">
            <b-form-input
              id="surname"
              placeholder="Jonathan"
              required
              v-model="receiver.surname"
            ></b-form-input>
          </b-form-group>
          <b-form-group
            i
            d="lastname-group"
            label-for="lastname"
            label="Efternamn"
          >
            <b-form-input
              id="lastname"
              placeholder="Luxman"
              v-model="receiver.lastname"
              required
            ></b-form-input>
          </b-form-group>
          <b-form-group
            id="street-group"
            label="Gata och Husnummer"
            label-for="street"
          >
            <b-form-input
              id="street"
              placeholder="Kungstorget 23"
              v-model="receiver.street"
              required
            ></b-form-input>
          </b-form-group>
          <b-form-group
            id="postNumber-group"
            label="Postadress"
            label-for="postAdress"
          >
            <b-form-input
              id="postAdress"
              required
              placeholder="41511"
              v-model="receiver.postAdress"
            ></b-form-input>
          </b-form-group>
          <b-form-group id="city" label="Ort" label-for="city">
            <b-form-input
              id="city"
              required
              placeholder="Gothenburg"
              v-model="receiver.city"
            ></b-form-input>
          </b-form-group>
          <b-form-group
            id="telephone"
            label="Mobilnummer"
            label-for="telephone"
          >
            <b-form-input
              id="telephone"
              placeholder="07XXXXXXX"
              required
              v-model="receiver.telephone"
            ></b-form-input>
          </b-form-group>
          <b-form-group
            id="email-group"
            label="Email adress"
            label-for="email-adress"
            v-model="receiver.email"
          >
            <b-form-input
              id="email-adress"
              type="email"
              placeholder="JonathanLuxman@email.com"
              required
              v-model="receiver.email"
            ></b-form-input>
          </b-form-group>
          <b-button type="submit" variant="primary">Beställ</b-button>
        </b-form>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: "Cart",
  data() {
    return {
      receiver: {
        surename: "",
        lastname: "",
        street: "",
        postAdress: "",
        city: "",
        telephone: "",
        email: "",
        payMethod: "",
        cardNumber: "",
        cardNumberName: "",
        paypalEmail: "",
        bitcoinAdress: ""
      },
      payMethodOptions: ["Visa", "Paypal", "Bitcoin", "Faktura"]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss"></style>
