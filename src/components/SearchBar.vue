<template>
  <form @submit.prevent="search">
    <div class="form-group">
      <input 
        v-model="foodName"
        id="search" 
        class="form-control" 
        placeholder="Search for a food" autofocus
        type="text" 
      >
    </div>
  </form>
</template>

<script>
export default {
  name: 'SearchBar',
  data() {
    return {
      foodName: '',
    };
  },
  methods: {
    search() {
      this.$emit('search', this.foodName);
    },
  }
};
</script>

<style scoped>
  .bmd-label-static {
    color: rgb(255, 255, 255);
  }

  .form-control,
  ::placeholder {
    font-size: 1.3rem;
    padding: 1em 5px;
    color: #fff;
    background-image: linear-gradient(0deg,#7a0820 2px,rgba(0,150,136,0) 0),linear-gradient(0deg,rgba(0,0,0,.26) 1px,transparent 0);
  }
</style>
