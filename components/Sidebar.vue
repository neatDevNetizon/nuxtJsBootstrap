<template>
    <div>
        <b-sidebar id="sidebar-left" title="MAP member" left shadow>
            <div class="px-3 py-2">
                <input type="text" placeholder="Fullname" class="form-control my-2">
                <input type="text" placeholder="Role" class="form-control my-2">
                <input type="email" placeholder="Email" class="form-control my-2">
                <input type="number" placeholder="Phone" class="form-control my-2">
                <div class="flex justify-content-center">
                    <button type="button" class="btn btn-success">Save</button>
                    <button type="button" class="btn btn-danger">Delete</button>
                </div>
            </div>
        </b-sidebar>
    </div>
</template>