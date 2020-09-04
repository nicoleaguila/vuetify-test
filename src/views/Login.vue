<template>
<div>
 <v-card width="420px" class="mx-auto my-auto mt-5">
    <v-card-title>
    <h1 class="mx-auto">login</h1>
    </v-card-title>
    <v-card-text>
      <v-form>
        <v-text-field label="userName" prepend-icon="mdi-account-circle"/> 
        <v-text-field 
        @click:append="showPassword = !showPassword" 
        label="password" 
        :type="showPassword ? 'text': 'password'" 
        prepend-icon="mdi-lock" 
        :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"/>
        </v-form>
    </v-card-text>
    <v-card-actions>
      <v-btn color="success">register</v-btn>
      <v-spacer></v-spacer>
      <v-btn color="info">login</v-btn>
    </v-card-actions>
    </v-card>  
    </div>
</template>

<script>
export default {
  data: () => ({
    showPassword: false
  }),
}
</script>

<style>

</style>