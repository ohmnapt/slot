<template>
  <div>
    <app-form>
      <template v-slot:help>
        <p>{{ help }}</p>
      </template>
      <template v-slot:field>
        <input type="text" placeholder="email" />
        <input type="text" placeholder="username" />
        <input type="password" placeholder="password" />
      </template>
      <template v-slot:button>
        <button type="submit">Submit</button>
      </template>
      <p>dummy text</p>
    </app-form>

    <app-form>
      <template v-slot:help>
        <p>Contact help text.</p>
      </template>

      <template v-slot:field>
        <input type="text" placeholder="name" />
        <input type="text" placeholder="message" />
      </template>

      <template v-slot:button>
        <button type="submit">Submit</button>
      </template>
    </app-form>
  </div>
</template>

<script>
import AppForm from "./components/Form.vue";
export default {
  name: "App",
  components: { AppForm },
  data() {
    return {
      help: "This is some help text.",
    };
  },
};
</script>
