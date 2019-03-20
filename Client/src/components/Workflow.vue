<template>
    <div id="workflow">
        <h3>Alur Tahap Pelelangan</h3>
        <v-stepper value="0">
            <v-stepper-header>
            <v-stepper-step step="1">Cari dan pilih figure</v-stepper-step>

            <v-divider></v-divider>

            <v-stepper-step step="2">Bid dengan harga yang sesuai</v-stepper-step>

            <v-divider></v-divider>

            <v-stepper-step step="3">Melakukan pembayaran</v-stepper-step>
            </v-stepper-header>
        </v-stepper>
    </div>
</template>

<script>
export default {
  name: 'Workflow',
}
</script>