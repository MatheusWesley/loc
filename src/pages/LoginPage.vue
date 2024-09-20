<template>
  <q-page padding>
    <q-form class="q-gutter-md">
      <q-input label="Nome" outlined>
        <template v-slot:append>
          <q-icon name="person" class="cursor-pointer">
          </q-icon>
        </template>
      </q-input>
      <q-input label="Email" outlined>
        <template v-slot:append>
          <q-icon name="email" class="cursor-pointer">
          </q-icon>
        </template>
      </q-input>
      <q-input label="Senha" v-model="password" outlined :type="isPwd ? 'password' : 'text'">
        <template v-slot:append>
          <q-icon :name="isPwd ? 'visibility_off' : 'visibility'" class="cursor-pointer" @click="isPwd = !isPwd" />
        </template>
      </q-input>
      <div class="column">
        <q-btn label="Confirmar" color="primary" />
      </div>
    </q-form>
  </q-page>
</template>

<script>
import { ref } from 'vue'

export default {
  name: "LoginPage",
  setup() {
    return {
      password: ref(""),
      isPwd: ref(true),
    };
  },
};
</script>
<style lang="css" scoped></style>
