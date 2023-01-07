<template>
  <div class="calculator">
    <div class="container">
      <h2>電卓</h2>
      <div class="row justify-content-center">{{ this.result }}</div>
      <div class="row justify-content-center my-3">
        <div class="col-3 d-flex justify-content-center">
          <button class="w-100 btn btn-outline-secondary">1</button>
        </div>
        <div class="col-3 d-flex justify-content-center">
          <button class="w-100 mx-auto btn btn-outline-secondary">2</button>
        </div>
        <div class="col-3 d-flex justify-content-center">
          <button class="w-100 mx-auto btn btn-outline-secondary">3</button>
        </div>
      </div>
      <div class="row justify-content-center my-3">
        <div class="col-3 d-flex justify-content-center">
          <button class="w-100 btn btn-outline-secondary">4</button>
        </div>
        <div class="col-3 d-flex justify-content-center">
          <button class="w-100 mx-auto btn btn-outline-secondary">5</button>
        </div>
        <div class="col-3 d-flex justify-content-center">
          <button class="w-100 mx-auto btn btn-outline-secondary">6</button>
        </div>
      </div>
      <div class="row justify-content-center my-3">
        <div class="col-3 d-flex justify-content-center">
          <button class="w-100 btn btn-outline-secondary">7</button>
        </div>
        <div class="col-3 d-flex justify-content-center">
          <button class="w-100 mx-auto btn btn-outline-secondary">8</button>
        </div>
        <div class="col-3 d-flex justify-content-center">
          <button class="w-100 mx-auto btn btn-outline-secondary">9</button>
        </div>
      </div>
      <div class="row justify-content-center my-3">
        <div class="col-3 d-flex justify-content-center">
          <button class="w-100 btn btn-outline-secondary">0</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {
    Calculator,
  },
})
export default class Calculator extends Vue {
  data(): object {
    return {
      result: "",
    };
  }
}
</script>
