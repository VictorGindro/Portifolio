<template>
    <v-container fluid>
        <v-card flat  class="mx-auto text-center">
            <div  class="text-h2">
                Lats 30 days
            </div>
            <v-sparkline :fill="true" :gradient="gradient" :padding="padding" :smooth="radius" :value="item.value"
                auto-draw color="#f0f">
                <template v-slot:label="item">
                    {{ item.value }}
                </template>
            </v-sparkline>
            <v-card-text>
                <div  class="text-h4">
                    Commits/Day
                </div>
            </v-card-text>
        </v-card>
    </v-container>
</template>
<script>
    export default {
        components: {
        },
        data: () => ({
            fill: true,
            gradient: ['#00c6ff', '#F0F', '#FF0'],
            padding: 8,
            radius: 10,
            item: {
                "value": [2, 2, 5, 9, 5, 10, 3, 5, 2, 7, 1, 8, 2, 9, 0, 15, 2, 5, 9, 5, 10, 3, 5, 0, 0, 1, 8, 2, 9, 0]
            },
        }),
    }
</script>