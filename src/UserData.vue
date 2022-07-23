<template>
  <form @submit.prevent="submitData">
    <div>
      <label>UserName</label>
      <input type="text" v-model="enterName" />
    </div>

    <div>
      <label>Age</label>
      <input type="number" v-model="enterAge" />
    </div>

    <div>
      <button>Add User</button>
    </div>
  </form>
</template>

<script>
export default {
  emits: ["addUser"],
  data() {
    return {
      enterName: "",
      enterAge: "",
    };
  },
  methods: {
    submitData() {
        this.$emit("addUser", this.enterName, this.enterAge);
    },
  },
};
</script>

<style></style>
