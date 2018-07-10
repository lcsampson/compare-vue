<template>
  <transition name="modal">
    <div class="modal-mask" v-on:click="$emit('close')">
      <div class="modal-wrapper">
        <div class="modal-container">
          <slot name="header">Header</slot>
          <button class="modal-default-button" v-on:click="$emit('close')">Close</button>
        </div>
      </div>
    </div>
  </transition>
</template>

<style>
    .modal-mask {
        position: fixed;
        z-index: 9998;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, .5);
        display: table;
        transition: opacity .4s ease;
    }

    button{
        border: none;
        background: #F44336;
        color: #fff;
        padding: 10px;
    }
    .modal-wrapper {
        display: table-cell;
        vertical-align: middle;
    }

    .modal-container {
        width: 300px;
        margin: 0px auto;
        padding: 20px 30px;
        min-height: 35px;
        background-color: #fff;
        border-radius: 2px;
        box-shadow: 0 2px 8px rgba(0, 0, 0, .33);
        transition: all .2s ease;
        font-family: Helvetica, Arial, sans-serif;
    }

    .modal-default-button {
        float: right;
    }
    .modal-enter {
      opacity: 0;
    }

    .modal-leave-active {
      opacity: 0;
    }

    .modal-enter .modal-container,
    .modal-leave-active .modal-container {
        -webkit-transform: scale(0.95);
        transform: scale(0.95);
    }
</style>
<script>

export default {
  name: 'modal'
}
</script>