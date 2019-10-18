<template>
  <div>
    <div class="container page">
      <div class="row">
        <div class="col-md-6 offset-md-3 col-xs-12">
          <form>
            <fieldset class="form-group">
              <input
                class="form-control form-control-lg"
                type="text"
                v-model="conjugation"
                placeholder="Conjugate"
              />
            </fieldset>
            <button
              @click="conjugaison()"
              class="btn btn-lg btn-primary pull-xs-right"
            >
              Conjugate
            </button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";

@Component
export default class Conjugaison extends Vue {
  conjugation = "";

  conjugaison() {
    console.log(this.conjugation);
  }
}
</script>
