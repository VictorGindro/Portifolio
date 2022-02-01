<template>
    <v-container>
        <v-row v-for="n in 2" :key="n">
            <v-responsive width="56" cols="12" justify-space-around wrap v-for="n in 3" :key="n">
                <v-col class="mb-5">
                    <Card />
                </v-col>
            </v-responsive>
        </v-row>
        <div class="text-center">
            <v-pagination color="teal" v-model="page" :length="6"></v-pagination>
        </div>
    </v-container>
</template>
<script>
    import Card from '../components/Card';

    export default {
        name: 'App',

        components: {
            Card,
        },

        data: () => ({
            page:1,
        }),
    };
</script>
<style scoped>
    /*{"Teal":"008080","Rebecca Purple":"663399","Navajo White":"f6d8ae","Cafe Noir":"573c23"}*/
</style>