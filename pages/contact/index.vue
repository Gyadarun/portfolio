<template>
    <div class="contact-form">
     <form name="contact" action="" method="post" netlify>
     <input type="hidden" name="form-name" value="contact" />
       
        <input class="form-field" name="name" id="name" placeholder="Nom" />
      
        <input class="form-field" name="email" id="email" placeholder="E-mail" />
       
        <textarea class="form-field" name="message" id="message" placeholder="Votre message"></textarea>

        <button class="form-button">Envoyer</button>
      
      </form>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.contact-form {
  margin: 0 auto;
  width: 30rem;
}
input, textarea {
  width: 100%;
}
input {
  height: 30px;
}
textarea {
  height: 120px;
}
.form-field {
  margin: 10px;
}
.form-button {
  display: block;
  margin: 0 auto;
}
</style>