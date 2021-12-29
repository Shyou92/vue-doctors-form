<template>
  <div id="app">
    <Form @isUserCreated="createUser($event)" />
    <ClientCreated @userCreated="closePopup()" :userCreated="userCreated" />
  </div>
</template>

<script>
import Form from './views/Form.vue';
import ClientCreated from './components/ClientCreated.vue';

export default {
  name: 'App',
  components: { Form, ClientCreated },
  data() {
    return {
      userCreated: false,
    };
  },
  methods: {
    createUser(userCreated) {
      this.userCreated = userCreated;
    },
    closePopup() {
      this.userCreated = false;
    },
  },
};
</script>

<style></style>
