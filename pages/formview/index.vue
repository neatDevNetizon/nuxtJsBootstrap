<template>
    <div class="d-flex justify-content-between">
        <Sidesection />
        <Form :formview="example"/>
    </div>
</template>

<script>
  import FormTable from '../../components/Form.vue'

  export default {
    name: 'post-container',
    components: { FormTable },
    data () {
      return {
        example: [
            {
                id: 1,
                field1: "9/19/2021",
                field2: true,
                field3: "Member Name",
                field4: 'Member Name',
                field5: 'Something'
            },
            {
                id: 2,
                field1: "9/19/2021",
                field2: true,
                field3: "Member Name",
                field4: 'Member Name',
                field5: 'Something'
            },
            {
                id: 3,
                field1: "9/19/2021",
                field2: false,
                field3: "Member Name",
                field4: 'Member Name',
                field5: 'Something'
            },
            {
                id: 4,
                field1: "9/19/2021",
                field2: true,
                field3: "Member Name",
                field4: 'Member Name',
                field5: 'Something'
            }
        ]
      }
    }
  }
</script>
