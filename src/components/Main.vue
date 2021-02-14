<template>
  <div>

    <v-card class="mb-8">
      <v-toolbar flat>
        <v-toolbar-title>Narrow by region</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-col
                class="d-flex"
                cols="12"
                sm="6"
        >
          <v-select
                  :items="regions"
                  label="Select region"
          ></v-select>
        </v-col>
      </v-toolbar>
    </v-card>

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