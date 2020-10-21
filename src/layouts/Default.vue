<template>
  <div class="layout">
    <list></list>
  </div>
</template>
<script>
  import List from "@/views/Lists.vue"
  import ListCreator from "@/views/ListCreator.vue"
  import { mapGetters } from "vuex";
  export default {
    components: {
      List,
      ListCreator
    },
    computed: {
      ...mapGetters({
        user: "user"
      })
    }
  };
</script>
