<template>
    <div class="w-100">
        <div class="d-flex justify-content-between p-2 bg-light align-items-center">
            <ul class="breadcrumb">
                <li><NuxtLink to="/account">UserName</NuxtLink><span class="divider">/</span></li>
                <li class="active">Fromview</li>
            </ul>
            <div class="d-flex justify-content-between">
                <div class="mx-2"><NuxtLink to="/#" class="btn btn-success">Save</NuxtLink></div>
                <div class="mx-2"><NuxtLink to="/#" class="btn btn-primary">Submit</NuxtLink></div>
                <div class="mx-2"><NuxtLink to="/#" class="btn btn-secondary">Preview</NuxtLink></div>
                <div class="mx-2"><NuxtLink to="/#" class="btn btn-warning">Setting</NuxtLink></div>
            </div>
        </div>
        <div class="p-2">
            <h6 class="text-success">Basic</h6>
            <div class="border d-flex px-4 py-2 align-items-end">
                <input type="text" class="form-control mx-2" id="validationCustom03" placeholder="Your Company" required>
                <input type="text" class="form-control mx-2" id="validationCustom03" placeholder="Our Company" required>
                <input type="text" class="form-control mx-2" id="validationCustom03" placeholder="suffix ex Deal" required>
                <input type="text" class="form-control mx-2 h-75" id="validationCustom03" placeholder="Values we share" required>
            </div>
            <h6 class="text-success">Team</h6>
            <div class="border d-flex px-4 py-2 align-items-end">
                <b-button class="btn btn-success">+</b-button>
                <label class="mx-2">Name 1</label>
                <label class="mx-2">Name 2</label>
                <label class="mx-2">Name 3</label>
            </div>
            <h6 class="text-success">Task</h6>
            <div class="border px-4 py-2 align-items-end h-300 overflow-auto">
                <b-button class="btn btn-success">+</b-button>
                <table class="table table-sm table-striped table-hover">
                    <thead>
                        <tr>
                            <th scope="col">Date</th>
                            <th scope="col">Completed</th>
                            <th scope="col">Owner(you)</th>
                            <th scope="col">Owner(we)</th>
                            <th scope="col">Note</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr v-for="items in formview" v-bind:key="items.id">
                            <td scope="row">{{items.field1}}</td>
                            <td><input type="radio" :checked="items.field2"></td>
                            <td>{{items.field3}}</td>
                            <td>{{items.field4}}</td>
                            <td>{{items.field5}}</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
    </div>
</template>

<style lang="css" scoped>
    .h-75{
        height: 100px!important;
    }
    .h-300{
        height: 300px;
    }
</style>

<script>
    export default {
        name: 'post',
        props: ['formview']
    }
</script>
