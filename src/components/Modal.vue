<template>
    <div class="backdrop">
        <div class="modal" :class="{ sale: themeProp === 'sale'}">
            <h1>{{fordyBind}}</h1>
            <p>{{textFordyBind}}</p> 
        </div>
    </div>
</template>

<script>
export default {
   props: ['fordyBind','textFordyBind', 'themeProp']
}
</script>


<style>
    .modal {
        width: 400px;
        padding: 20px;
        margin: 100px auto;
        background: white;
        border-radius: 10px;
    }
    .backdrop {
        top: 0;
        position: fixed;
        background: rgba(0, 0, 0, 0.5);
        width: 100%;
        height: 100%;
    }
    .modal h1 {
       color: #03cfb4;
       border: none;
       padding: 0;
    }
    .modal p {
        font-style: normal;
    }

    .modal.sale {
        background:crimson;
        color: white;
    }
    .modal.modal.sale.h1 {
        color: white;
    }
</style>