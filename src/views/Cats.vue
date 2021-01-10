<template>
  <div>
      <h1>Cats for Adoption</h1>
    <b-table striped hover :items="cats">
        <template #cell(name)="data">
        <router-link
         :to="`/pets/${data.index}`">{{ data.value }}</router-link>
      </template>
    </b-table>
  </div>
</template>

<script>

export default {
  data () {
    return {
      cats: [
        { Name: 'Henry', Breed: 'Tabby', Gender: 'Male', Age: '19', Color: 'orange/white' },
        { Name: 'Roger', Breed: 'Tabby', Gender: 'Female', Age: '9', Color: 'black' },
        { Name: 'Kitkat', Breed: 'Bombay', Gender: 'Female', Age: '6', Color: 'white' },
        { Name: 'Fish', Breed: 'tuxedo', Gender: 'Male', Age: '20', Color: 'gray' }
      ]
    }
  }
}
</script>

<style lang="stylus"></style>
