<template>
  <span>
    <UserInput />
    <UserDetails v-for="(user,i) in users" :key="i" :name="user.name" :lastname="user.lastname" />
  </span>
</template>

<script>
import UserInput from "@/components/UserInput";
import UserDetails from "@/components/UserDetails";
export default {
  components: { UserInput, UserDetails },
  data() {
    return {
      users: [
        { name: "Jane", lastname: "Doe" },
        { name: "Joe", lastname: "Dalton" },
        { name: "Luke", lastname: "Skywalker" },
        { name: "Bruce", lastname: "Willis" },
      ],
    };
  },
};
</script>


<style>
</style>