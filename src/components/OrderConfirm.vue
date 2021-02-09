<template>
  <div>
  <div class="OrderConfirm">
    <h1>Beställningen har Behandlats</h1>
    <p> Nummer 0123456789 </p>
    <h2> Du kommer få din beställning : </h2>
        <p> Mån 1 mars - Tors 5 mars </p>

        <h3> Genomför registeringen </h3>
        <p> Spara dina uppgifter för framtida köp. Du behöver bara lägga till ett lösenord. </p>

    <p> Epostadress: info@.com</p>

    <p> Jag har haft möjligheter att läsa och jag förstår Sekretess - och Coockiespolicyn. </p>

    <h5>Product</h5>
  <b-img src="https://picsum.photos/300/150/?image=41" fluid alt="Product image"></b-img>
</div>

 <b-list-group-item class="d-flex justify-content-between align-items-center">
      <b-icon icon="check-circle" scale="2" variant="success"></b-icon>
    </b-list-group-item>


 <b-form @submit.stop.prevent>
    <label for="text-password">Lösenord</label>
    <b-form-input type="password" id="text-password" aria-describedby="password-help-block"></b-form-input>
    <b-button variant="dark">Bekräfta</b-button>
   </b-form>
<b-list-group>
    
   

  <b-container class="bv-example-row">
  <b-row>
    <b-col>Fraktsätt</b-col>
    <b-col>Standardleverans till hemmet.</b-col>
    
  </b-row>
</b-container>


<b-card-group deck>
    <b-card border-variant="dark" header="Leveransadress" align="center">
        <b-card-text>Här kommer info om kundens leveransadress!</b-card-text>
      </b-card>
    </b-card-group>

<b-container class="bv-example-row">
  <b-row>
    <b-col>Betalsätt</b-col>
    <b-col>PAYPAL</b-col>
    
  </b-row>
</b-container>

<b-card-group deck>
    <b-card border-variant="dark" header="Kontaktuppgifter" align="center">
        <b-card-text>Här kommer info om kundens kontaktuppgifter såsom telefonnummer, e-post osv!</b-card-text>
      </b-card>
    </b-card-group>

    <b-card-group deck>
    <b-card border-variant="dark" header="Fördelning" align="center">
        <b-card-text>Här kommer info om produktens pris, fraktavgift, totalpris och moms!</b-card-text>
      </b-card>
    </b-card-group>


    <b-form-rating v-model="rate" variant="warning" class="mb-2"></b-form-rating>
    <p class="mt-2">Value: {{ rate }}</p>
    <b-list-group-item class="d-flex justify-content-between align-items-center">
      
    </b-list-group-item>

    <div>
  
  <b-button href="#">Tillbaka till Hem</b-button>
</div>
  
</template>

<script>
  export default {
    data() {
      return {
        rate: null
      }
    }
  }
</script>