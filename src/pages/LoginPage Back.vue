<template>
  <q-page padding>
    <q-form>
      <div class="q-nb-nd">
        <q-input model-value="" label="Nome" outlined />
      </div>
      <div class="rom- q-col-gutter-x-nd">
        <q-input label="Email" outlined>
          <template v-slot:append>
            <q-icon name="email" class="cursor-pointer">
            </q-icon>
          </template>
        </q-input>
      </div>
      <password-input />
      <div class="column">
        <q-btn label="Confirmar" color="primary" />
      </div>

    </q-form>
  </q-page>
</template>

<script>
import PasswordInputVue from 'src/components/PasswordInput.vue'
import PasswordInput from 'src/components/PasswordInput.vue'
export default {
  components: { PasswordInput },
  name: 'LoginPage',
  setup() {

    return {

    }
  }
}
</script>
<style lang="css" scoped></style>
