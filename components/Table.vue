<template>
    <div class="w-100">
        <div class="d-flex justify-content-between p-2 bg-light">
            <ul class="breadcrumb">
                <li><NuxtLink to="/account">UserName</NuxtLink><span class="divider">/</span></li>
                <li class="active">Overview</li>
            </ul>
            <div><NuxtLink to="/formview" class="btn btn-success">Go To FormView</NuxtLink></div>
        </div>
        <div class="p-2">
            <table class="table table-sm table-striped table-hover">
                <thead>
                    <tr>
                        <th scope="col">Vendor</th>
                        <th scope="col">Task Completed</th>
                        <th scope="col">Next</th>
                        <th scope="col">Days Focus day</th>
                        <th scope="col">Actions</th>
                    </tr>
                </thead>
                <tbody>
                    <tr v-for="items in example" v-bind:key="items.id">
                        <td scope="row">{{items.field1}}</td>
                        <td>{{items.field2}}</td>
                        <td>{{items.field3}}</td>
                        <td>{{items.field4}}</td>
                        <td class="d-flex align-items-center"><b-form-checkbox 
                            name="checkbox-1"
                            value="accepted"
                            unchecked-value="not_accepted"
                            >
                            </b-form-checkbox>
                            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-trash " role="button"  viewBox="0 0 16 16">
                                <path d="M5.5 5.5A.5.5 0 0 1 6 6v6a.5.5 0 0 1-1 0V6a.5.5 0 0 1 .5-.5zm2.5 0a.5.5 0 0 1 .5.5v6a.5.5 0 0 1-1 0V6a.5.5 0 0 1 .5-.5zm3 .5a.5.5 0 0 0-1 0v6a.5.5 0 0 0 1 0V6z"/>
                                <path fill-rule="evenodd" d="M14.5 3a1 1 0 0 1-1 1H13v9a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V4h-.5a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1H6a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1h3.5a1 1 0 0 1 1 1v1zM4.118 4 4 4.059V13a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1V4.059L11.882 4H4.118zM2.5 3V2h11v1h-11z"/>
                            </svg>
                        </td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</template>
<script>
  export default {
    name: 'post',
    props: ['example']
  }
</script>
