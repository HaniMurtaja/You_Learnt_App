<template>
    <div class="contact-us">
        <PagesHero title="Contact Us" />
        <v-container>
            <div class="page-content pt-6 pb-10 mt-16">
                <div class="text-center mb-10">
                    <h3>
                        Our experts will help you
                    </h3>
                    <p>
                        If you have question, leave your request: we will be happy to answer all your questions.
                    </p>
                </div>
                <v-row>
                    <v-col cols="12" md="2" />
                    <v-col cols="12" md="8">
                        <v-form>
                            <v-row>
                                <v-col cols="12" md="6">
                                    <v-text-field
                                        label="Email"
                                        hide-details
                                        clearable
                                        outlined
                                        dense
                                    />
                                </v-col>
                                <v-col cols="12" md="6">
                                    <v-text-field
                                        label="Name"
                                        hide-details
                                        clearable
                                        outlined
                                        dense
                                    />
                                </v-col>
                                <v-col cols="12" md="6">
                                    <v-text-field
                                        label="Phone Number"
                                        hide-details
                                        clearable
                                        outlined
                                        dense
                                    />
                                </v-col>
                                <v-col cols="12" md="6">
                                    <v-text-field
                                        label="Subject"
                                        hide-details
                                        clearable
                                        outlined
                                        dense
                                    />
                                </v-col>
                                <v-col cols="12">
                                    <v-text-field
                                        outlined
                                        hide-details
                                        clearable
                                        label="Your Message Here"
                                        type="text"
                                        height="150"
                                    />
                                </v-col>
                              <v-btn class="mx-auto px-8 mt-4" x-large elevation="0" color="secondary"> Send Message </v-btn>
                            </v-row>
                        </v-form>
                      <div class="d-flex mt-8 align-center justify-center">
                        <p class="textdark--text px-0 py-0 font-weight-medium my-0 mx-3">Do you want to talk to our support team?</p>
                        <v-btn class="px-10 primary--text" large outlined> <v-icon class="pe-2" >fas fa-headset</v-icon> Live Chat</v-btn>
                      </div>
                    </v-col>
                    <v-col cols="12" md="2" />
                </v-row>
            </div>
        </v-container>
    </div>
</template>

<style lang="scss" scoped>
.contact-us {
  h3 {
    color: #212529;
    font-size: 24px;
    font-weight: 500;
  }
  p {
    font-size: 14px;
    color: #212529;
    margin-top: 12px;
  }
}
</style>
