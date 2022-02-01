<template>
    <v-card class="mx-5" color="teal" dark max-width="400">
        <v-card-title>
            <v-icon large left>
                mdi-git
            </v-icon>
            <span class="text-h6 font-weight-light"> Repository </span>
        </v-card-title>

        <v-card-text class="text-h5 font-weight-bold">
            Lorem ipsum dolor sit amet consectetur adipisicing elit.
        </v-card-text>

        <v-card-actions>
            <v-list-item class="grow">

                <v-row align="center" justify="start">
                    <v-icon class="mr-1">
                        mdi-source-branch
                    </v-icon>
                    <span class="subheading mr-2">branch</span>
                    <v-spacer />
                    <span class="mr-1">
                        <v-icon>mdi-code-array</v-icon>
                    </span>
                    <v-spacer />
                    <v-icon class="mr-1">
                        mdi-calendar-cursor
                    </v-icon>
                    <span class="subheading">16/12/22</span>
                </v-row>
            </v-list-item>
        </v-card-actions>
    </v-card>
</template>
<style scoped>
/*{"Teal":"008080","Rebecca Purple":"663399","Navajo White":"f6d8ae","Cafe Noir":"573c23"}*/
</style>