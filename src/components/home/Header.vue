<template>
    <v-sheet
        :height="sheetHeight"
    >
        <v-container class="fill-height">
            <v-row
                align="center"
                justify="center"
            >
                <h1 class="text-center display-1 hidden-xs-only">Vuetify hidden-xs-only</h1>
                <h1 class="text-center display-1 hidden-sm-and-up">Vuetify hidden-sm-and-up</h1>
            </v-row>
            
        </v-container>
    </v-sheet>
</template>

<script>
export default {
    computed:{
        sheetHeight(){
            switch (this.$vuetify.breakpoint.name) {
                case 'xs': return '200px'
                case 'sm': return '300px'
                case 'md': return '300px'
                case 'lg': return '300px'
                case 'xl': return '350px'
            }
            return '300px'
        }
    }
}
</script>

<style>

</style>