<template>
  <div id="app">
    <Form />
    <ClientCreated />
  </div>
</template>

<script>
import Form from './views/Form.vue';
import ClientCreated from './components/ClientCreated.vue';

export default {
  name: 'App',
  components: { Form, ClientCreated },
};
</script>

<style></style>
