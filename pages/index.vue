<template>
    <div class="content">
        <div class="button_section">
            <NuxtLink to="/tableview" class="btn btn-success">Go To TableView</NuxtLink>
        </div>
        <div class="hero-unit well p-2 h-full">
            <h1 class="text-center text-primary">Welcome</h1>
            <p class="text-center text-success">Click the above button link to TableView</p>
        </div>
    </div>
</template>

<style>
    .button_section{
        display: flex;
        justify-content: flex-end;
        margin-top: 10px;
        margin-right: 10px;
        margin-left: 10px;
    }
    button a{
        color: white;
    }
    button a:hover{
        color: white;
        text-decoration: none;
    }
    .well{
        background: #eeeeee;
        border-radius: 5px;
        margin-top: 30px;
        margin-right: 10px;
        margin-left: 10px;
    }
</style>