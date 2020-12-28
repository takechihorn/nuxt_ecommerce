<template>
  <section className="checkout-wrapper">
    <AmplifyAuthenticator>
      <Elements stripe={stripePromise}>
        <section>
          <h2>Time to Checkout</h2>
          <CheckForm/>
        </section>
      </Elements>
    </AmplifyAuthenticator>
  </section>
</template>

<script>
export default {

}
</script>

<style>

</style>
