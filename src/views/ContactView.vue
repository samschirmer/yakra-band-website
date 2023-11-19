<template>
  <div class="contact content green">
    <h1 class="green">Contact</h1>
    <div>
      <p>
        Send all hate mail to {{ email }}
      </p>
      <p>
        This is a one-man band, so playing live is an impossibility. 
      </p>

    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: atob("c2Ftc2NoaXJtZXJAZ21haWwuY29t")
    };
  },
}
</script>

<style>
@media (min-width: 1024px) {
  .contact {
    min-height: 100vh;
    max-width: 800px;
    margin: auto;
    padding-top: 60px;
    padding-bottom: 100px;
  }
}
</style>
