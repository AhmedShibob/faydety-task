<template>
  <section class="loans">
   <div class="container">
        <Loan v-for="loan in 5" :key="loan + 'loan'" />
   </div>
  </section>
</template>

<script>
import Loan from "./loan/loan";
export default {
  components: {
    Loan,
  },
};
</script>
