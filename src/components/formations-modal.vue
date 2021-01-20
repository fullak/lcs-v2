<template>
  <transition name="modal">
    <div class="modal-mask">
      <div class="modal-wrapper">
        <div class="modal-container bg-primary">
          <button class="modal-default-button text-white" @click="$emit('close')">
            X
          </button>

          <div class="modal-header">
            <h1 class="text-white text-4xl text-center">Title test</h1>
          </div>

          <div class="modal-body">
            <slot name="body">
              <iframe class="mt-10 mx-auto" width="860" height="515" src="https://www.youtube.com/embed/GqVfqOkoEhs" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </slot>
          </div>

          <div class="modal-footer">
            <slot name="footer">
              <p class="px-20 mt-10 text-white">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad adipisci aliquam, culpa delectus deserunt
                enim exercitationem incidunt iste mollitia officiis omnis possimus quas qui quod similique sint velit
                veniam voluptates.
                <br> <br>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad adipisci aliquam, culpa delectus deserunt
                enim exercitationem incidunt iste mollitia officiis omnis possimus quas qui quod similique sint velit
                veniam voluptates.
                <br> <br>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad adipisci aliquam, culpa delectus deserunt
                enim exercitationem incidunt iste mollitia officiis omnis possimus quas qui quod similique sint velit
                veniam voluptates.
                <br> <br>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad adipisci aliquam, culpa delectus deserunt
                enim exercitationem incidunt iste mollitia officiis omnis possimus quas qui quod similique sint velit
                veniam voluptates.
                <br> <br>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad adipisci aliquam, culpa delectus deserunt
                enim exercitationem incidunt iste mollitia officiis omnis possimus quas qui quod similique sint velit
                veniam voluptates.
                <br> <br>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad adipisci aliquam, culpa delectus deserunt
                enim exercitationem incidunt iste mollitia officiis omnis possimus quas qui quod similique sint velit
                veniam voluptates.
              </p>
            </slot>
          </div>
        </div>
      </div>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'Modal',
}
</script>

<style>
.modal-mask {
  position: fixed;
  z-index: 9998;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  display: table;
  transition: opacity 0.3s ease;
}

.modal-wrapper {
  display: table-cell;
  vertical-align: middle;
}

.modal-container {
  width: 80%;
  height: 90%;
  margin: 0px auto;
  padding: 20px 30px;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.33);
  transition: all 0.3s ease;
  font-family: Helvetica, Arial, sans-serif;
  overflow-y: auto;
}

.modal-header {
  margin-top: 0;
}

.modal-body {
  margin: 20px 0;
}

.modal-default-button {
  float: right;
}

/*
 * The following styles are auto-applied to elements with
 * transition="modal" when their visibility is toggled
 * by Vue.js.
 *
 * You can easily play with the modal transition by editing
 * these styles.
 */

.modal-enter {
  opacity: 0;
}

.modal-leave-active {
  opacity: 0;
}

.modal-enter .modal-container,
.modal-leave-active .modal-container {
  -webkit-transform: scale(1.1);
  transform: scale(1.1);
}

</style>