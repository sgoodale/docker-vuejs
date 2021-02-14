<template>
    <v-navigation-drawer
            permanent
            absolute
            expand-on-hover
    >
        <v-list>
            <v-list-item class="px-2">
                <v-list-item-avatar>
                    <v-img :src="require('../assets/logo.png')" aspect-ratio="1"></v-img>
                </v-list-item-avatar>
            </v-list-item>

            <v-list-item link class="nav-bar-title">
                <v-list-item-content>
                    <v-list-item-title class="title">
                        BC Covid-19 Dashboard
                    </v-list-item-title>
                    <v-list-item-subtitle>Relevant stats now.</v-list-item-subtitle>
                </v-list-item-content>
            </v-list-item>
        </v-list>

        <v-divider></v-divider>

        <v-list
                nav
                dense
        >
            <v-list-item link>
                <v-list-item-icon>
                    <v-icon>mdi-folder</v-icon>
                </v-list-item-icon>
                <v-list-item-title>My Files</v-list-item-title>
            </v-list-item>
            <v-list-item link>
                <v-list-item-icon>
                    <v-icon>mdi-account-multiple</v-icon>
                </v-list-item-icon>
                <v-list-item-title>Shared with me</v-list-item-title>
            </v-list-item>
            <v-list-item link>
                <v-list-item-icon>
                    <v-icon>mdi-star</v-icon>
                </v-list-item-icon>
                <v-list-item-title>Starred</v-list-item-title>
            </v-list-item>
        </v-list>
    </v-navigation-drawer>
</template>

<script>
    export default {
        name: "NavBar"
    }
</script>

<style scoped>

</style>