<template>
  <div>
    <pet-table :species="'Cats'" :pets="cats"/>
  </div>
</template>

<script>
import { mapState } from 'vuex'
import PetTable from '@/components/PetTable'
export default {
  data () {
    return { }
  },
  components: {
    'pet-table': PetTable
  },
  computed: {
    ...mapState([
      'cats'
    ])
  }
}
</script>
