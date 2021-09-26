<template>
    <div class="d-flex justify-content-between">
        <Sidesection />
        <Table :example="example"/>
    </div>
</template>

<script>
  import Table from '../../components/Table.vue'
  export default {
    name: 'post-container',
    components: { Table },
    data () {
      return {
        example: [
            {
                id: 1,
                field1: "Giacomo Guilizzoni 1",
                field2: 22,
                field3: "Something Something",
                field4: 'asdfasdf',
                field5: 'asdfadf'
            },
            {
                id: 2,
                field1: "Giacomo Guilizzoni 1",
                field2: 23,
                field3: "Something Something",
                field4: 'asdfasdf',
                field5: 'asdfadf'
            },
            {
                id: 3,
                field1: "Giacomo Guilizzoni 1",
                field2: 24,
                field3: "Something Something",
                field4: 'asdfasdf',
                field5: 'asdfadf'
            },
            {
                id: 4,
                field1: "Giacomo Guilizzoni 1",
                field2: 25,
                field3: "Something Something",
                field4: 'asdfasdf',
                field5: 'asdfadf'
            }
        ]
      }
    }
  }
</script>
