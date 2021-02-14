<template>
    <v-row class="pl-3 pr-3">

        <v-col
                v-for="n in Number(numCards)"
                :key="n"
        >

            <slot :name="'card-' + n"/>

        </v-col>

    </v-row>
</template>

<script>
    export default {
        name: 'CardRow',
        components: {},
        data: () => ({
            //
        }),
        props: ['numCards']
    }
</script>