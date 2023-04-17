<template>
  <v-container class="fill-height">
    <v-responsive class="d-flex align-center text-center fill-height">
      <v-img
        contain
        height="300"
        src="@/assets/logo.svg"
      />
      <v-row class="d-flex align-center justify-center">
        <v-col cols="4">
          <v-text-field
            v-model="value"
            color="primary"
            variant="outlined"
            density="comfortable"
            label="That is a bug"
          >
            <v-icon slot="prependInner" class="mr-2" color="red" icon="mdi-circle" />
          </v-text-field>
        </v-col>
        <v-col cols="4">
          <v-text-field
            v-model="value"
            color="primary"
            variant="outlined"
            density="comfortable"
            label="Good way"
          >
            <template v-slot:prepend-inner>
              <v-icon color="orange" icon="mdi-circle" />
            </template>
          </v-text-field>
        </v-col>
        <v-col cols="4">
          <v-text-field
            v-model="value"
            color="primary"
            variant="outlined"
            density="comfortable"
            label="No bug but I want a red circle"
            prepend-inner-icon="mdi-circle"
          >
          </v-text-field>
        </v-col>
      </v-row>

    </v-responsive>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      value: '',
    }),
  }

  //
</script>
