<template>
  <div>
    <Hero />
    <FilterSearch />
    <Loans />
    <FilterSearchPhone />
  </div>
</template>

<script>
import Hero from "../../components/hero/hero";
import FilterSearch from "../../components/filterSearch/filterSearch";
import Loans from "../../components/loans/loans";
import FilterSearchPhone from "../../components/filterSearchPhone/filterSearchPhone";

export default {
  name: "Home",
  components: { Hero, FilterSearch, Loans, FilterSearchPhone  },
};
</script>
