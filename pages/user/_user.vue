<template>
  <v-layout>
    <v-flex text-xs-center>
      {{$route.params.user}} <br>
      {{$auth.user.user.username}}
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  middleware: ['auth'],
}
</script>
