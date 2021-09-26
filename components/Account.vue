<template>
    <div class="w-100">
        <div class="d-flex justify-content-between p-2 bg-light">
            <ul class="breadcrumb">
                <li><NuxtLink to="/account">UserName</NuxtLink><span class="divider">/</span></li>
                <li class="active">Account</li>
            </ul>
            <div><NuxtLink to="/formview" class="btn btn-success">Save</NuxtLink></div>
        </div>
        <div class="d-flex p-2">
            <div class="upload">
                <input type="file">
            </div>
            <div class="mx-4">
                <input type="text" class="form-control my-2 w-200" id="validationCustom03" placeholder="Username" required>
                <input type="text" class="form-control my-2 w-200" id="validationCustom03" placeholder="Firstname" required>
                <input type="text" class="form-control my-2 w-200" id="validationCustom03" placeholder="Lastname" required>
            </div>
        </div>
        <div class="p-2">
            <input type="text" class="form-control h-400" id="validationCustom03" placeholder="Some Content Area" required>
        </div>
    </div>
</template>

<style scoped>
    input:focus{
        outline: none;
    }
    .upload{
        border: 1px solid black;
    }
    .upload input{
        height: 200px;
        width: 200px;
        opacity: 0;
    }
    .w-200{
        width: 200%;
    }
    .h-400{
        height: 300px;
    }
</style>