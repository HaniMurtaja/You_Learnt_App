<template>
    <div class="faq">
        <PagesHero title="Faq" />
        <v-container>
            <div class="test-class pb-4 mt-16 pt-4">
                <div class="text-center mb-7" :class="$vuetify.breakpoint.mobile ? 'w-100' : 'w-50 mx-auto'">
                    <h2 class="font-weight-medium font-size mb-3 fs-32">
                        Getting Started Guide
                    </h2>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit. A alias aperiam, culpa delectus deleniti fugit id laboriosam molestias nemo.
                    </p>
                </div>
                <div class="mx-md-16 px-md-16">
                    <div class="mb-9">
                      <v-text-field
                          label="Search..."
                          hide-details
                          clearable
                          outlined
                          dense
                          class="w-50 mx-auto"
                      />
                    </div>
                    <FaqItem />
                    <FaqItem />
                    <FaqItem />
                </div>
            </div>
        </v-container>
    </div>
</template>

<script>
import FaqItem from '~/components/homeComponents/FaqItem'
export default { components: { FaqItem } }
</script>
<style>
@media screen and (max-width: 700px) {
  .w-50 {
    width: 100% !important;
  }
}
</style>
