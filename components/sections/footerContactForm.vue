<template>
  <v-form>
    <v-text-field label="Nombre" dense outlined></v-text-field>
    <v-text-field label="Email" dense outlined></v-text-field>
    <v-text-field label="Subject" dense outlined></v-text-field>
    <v-textarea
      dense
      label="Tu mensaje"
      auto-grow
      outlined
      rows="8"
      row-height="20"
    ></v-textarea>
    <v-btn outlined block color="primary">Enviar Mensaje</v-btn>
  </v-form>
</template>
