<template>
  <b-container>
    <b-form @submit.prevent="Onsubmit">
      <b-form-group id="surname-group" label-for="surname" label="Förnamn">
        <b-form-input id="surname" placeholder="John" required></b-form-input>
      </b-form-group>
      <b-form-group i d="lastname-group" label-for="lastname" label="Efternamn">
        <b-form-input id="lastname" placeholder="Doe"></b-form-input>
      </b-form-group>
      <b-form-group id="adress-group" label="Adress" label-for="adress">
        <b-form-input id="adress" placeholder="Kungstorget 23"></b-form-input>
      </b-form-group>
      <b-form-group
        id="postNumber-group"
        label="Postadress"
        label-for="postAdress"
      >
        <b-form></b-form>
      </b-form-group>
      <b-form-group
        id="email-group"
        label="Email adress"
        label-for="email-adress"
      >
        <b-form-input
          id="email-adress"
          type="email"
          placeholder="JohnDoe@email.com"
          required
        ></b-form-input>
      </b-form-group>
    </b-form>
  </b-container>
</template>

<script>
export default {
  name: "Cart"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss"></style>
