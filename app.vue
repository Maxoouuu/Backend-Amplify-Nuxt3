<script setup lang="ts">
import { Authenticator } from "@aws-amplify/ui-vue";
import { Auth } from "aws-amplify";
/* Import styles */
import "@aws-amplify/ui-vue/styles.css";

</script>
<template>
  <div>
    <Authenticator >
      <template v-slot="{user, signOut}">
        <h1>Hello {{ user.username }}</h1>
        <button @click="signOut">Sign Out</button>
      </template>
    </Authenticator>
  </div>
</template>
