<template>
    <div>
        <h1>Dogs for Adoption</h1>
       <b-table striped hover :items="dogs"></b-table>
    </div>
</template>

<script>
export default {
  data () {
    return {
      dogs: [
        { Name: 'Billy', Breed: 'Asian', Gender: 'Male', Age: '9', Color: 'gray' },
        { Name: 'Arrow', Breed: 'Golden Retriever', Gender: 'Female', Age: '4', Color: 'black' },
        { Name: 'Major', Breed: 'Asian', Gender: 'Female', Age: '6', Color: 'white' },
        { Name: 'Captain', Breed: 'Asian', Gender: 'Male', Age: '7', Color: 'gray' }
      ]
    }
  }
}
</script>
