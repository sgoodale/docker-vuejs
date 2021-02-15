<template>
  <div>

    <v-toolbar flat class="mt-8 mb-12 mt-sm-0 mb-sm-4">
      <v-row>
        <v-col cols="12" sm="8" md="9">
          <v-toolbar-title>Dashboard Title</v-toolbar-title>
        </v-col>
        <v-spacer></v-spacer>
        <v-col cols="12" sm="4" md="3">
          <v-select
                  :items="regions"
                  label="Select region"
                  class="region-selector mb-0"
          ></v-select>
        </v-col>
      </v-row>
    </v-toolbar>

    <Section>
      <CardRow
              num-cards="2"
      >

        <v-card slot="card-1"
                class="pa-3"
                outlined
                tile
                style="height: 250px;"
        >
          <v-list-item three-line>
            <v-list-item-content>
              <div class="overline mb-4">
                OVERLINE
              </div>
              <v-list-item-title class="headline mb-1">
                Headline 5
              </v-list-item-title>
              <v-list-item-subtitle>Greyhound divisely hello coldly fonwderfully</v-list-item-subtitle>
            </v-list-item-content>

            <v-list-item-avatar
                    tile
                    size="80"
                    color="grey"
            ></v-list-item-avatar>
          </v-list-item>

          <v-card-actions>
            <v-btn
                    outlined
                    rounded
                    text
            >
              Button
            </v-btn>
          </v-card-actions>
        </v-card>

        <v-card slot="card-2"
                class="pa-3"
                outlined
                tile
                style="height: 250px;"
        >
          Insert content here 2
        </v-card>

      </CardRow>
    </Section>

  </div>
</template>

<style>
  @import '../stylesheets/main.css';
</style>

<script>
  import Section from "../partials/Section";
  import CardRow from "../partials/CardRow";

  export default {
    name: 'Main',
    components: {
      CardRow,
      Section,
    },
    data: () => ({
      regions: ['Island Health', 'Fraser', 'Northern', 'Interior']
    }),
  }

</script>