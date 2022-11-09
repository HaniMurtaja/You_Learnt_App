<template>
    <div class="referral-link-page">
        <div class="header-referral-link mb-16">
            <v-container>
                <v-row class="py-4" align="center">
                    <v-col cols="12" md="6">
                        <div class="desc pe-md-4">
                            <h1 class="mb-5">
                                Invite your friend, and you'll both get USD 10
                            </h1>
                            <p>
                                You and your friend who joins YouLearnt by your referral link will get both of you 10$ in your wallets when he books the first package on YouLearnt.
                            </p>
                        </div>
                    </v-col>
                    <v-col cols="12" md="6">
                        <img width="100%" :src="require('../assets/images/img-referral-link.png')">
                    </v-col>
                </v-row>
                <div class="share-box">
                    <div class="content">
                        <h2 class="primary--text">
                            Share your link
                        </h2>
                        <p>
                            Lorem ipsum dolor sit amet, consetetur sadipscing elitr,
                        </p>
                        <div class="box mb-4">
                            <v-text-field
                                hide-details
                                clearable
                                outlined
                                dense
                                disabled
                                value="https://www.w3.org/Provider/Style/dummy.html"
                            />
                        </div>
                        <v-row justify="center">
                            <v-col cols="12" md="6">
                                <div class="d-flex align-center justify-space-between">
                                    <v-btn color="secondary" elevation="0">
                                        <v-icon class="me-2">
                                            fas fa-copy
                                        </v-icon>
                                        Copy link
                                    </v-btn>
                                    <div class="d-flex align-center">
                                        <span class="me-2">Share link</span>
                                        <div class="social-media-circle primary">
                                            <v-icon color="white" size="13">
                                                fab fa-facebook-f
                                            </v-icon>
                                        </div>
                                        <div class="mx-2 social-media-circle primary">
                                            <v-icon color="white" size="13">
                                                fab fa-twitter
                                            </v-icon>
                                        </div>
                                        <div class="social-media-circle primary">
                                            <v-icon color="white" size="13">
                                                fab fa-instagram
                                            </v-icon>
                                        </div>
                                    </div>
                                </div>
                            </v-col>
                        </v-row>
                    </div>
                </div>
            </v-container>
        </div>
        <br><br><br><br><br><br>
        <v-container>
            <div class="have-earned mt-7 mb-14">
                <v-row justify="center">
                    <v-col cols="12" md="6">
                        <div class="box px-md-5 py-md-5 px-3 py-3">
                            <h3 class="font-weight-medium mb-4">
                                You have earned <span class="primary--text">$0 USD</span>
                                in bounces this month
                            </h3>
                            <v-data-table
                                :headers="headers"
                                :items="earned_data"
                                :items-per-page="5"
                                class="elevation-0"
                            />
                        </div>
                    </v-col>
                </v-row>
            </div>
        </v-container>
    </div>
</template>

<script>
export default {
    data() {
        return {
            headers: [
                {
                    text: 'Date',
                    value: 'date',
                    align: 'start',
                },
                {
                    text: 'Email',
                    value: 'email',
                    align: 'center',
                },
                {
                    text: 'Status',
                    value: 'status',
                    align: 'end',
                },
            ],
            earned_data: [
                {
                    date: '15-04-2020',
                    email: 'test@gmail.net',
                    status: 'Active',
                },
                {
                    date: '15-04-2020',
                    email: 'test@gmail.net',
                    status: 'Active',
                },
                {
                    date: '15-04-2020',
                    email: 'test@gmail.net',
                    status: 'Active',
                },
                {
                    date: '15-04-2020',
                    email: 'test@gmail.net',
                    status: 'Active',
                },
                {
                    date: '15-04-2020',
                    email: 'test@gmail.net',
                    status: 'Active',
                },
                {
                    date: '15-04-2020',
                    email: 'test@gmail.net',
                    status: 'Active',
                },
                {
                    date: '15-04-2020',
                    email: 'test@gmail.net',
                    status: 'Active',
                },
            ],
        }
    },
}
</script>

<style lang="scss" scoped>
.referral-link-page {
  .header-referral-link {
    background-image: url("../assets/images/bg-affiliate-header.png");
    background-size: cover;
    .container {
      position: relative;
      .desc {
        h1 {
          @media screen and (max-width: 720px) {
            margin-top: 32px !important;
            font-size: 32px !important;
            line-height: 1.2;
          }
          color: #fff;
          font-weight: 500;
          font-size: 38px;
        }
        p {
          color: #fff;
          font-size: 16px;
        }
      }
      .share-box {
        width: 75%;
        @media screen and (max-width: 720px) {
          width: 94% !important;
        }
        transform: translate(-50%,-50%)!important;
        left: 50%;
        top: 100%;
        position: absolute;
        .content {
          border-radius: .3rem!important;
          background: #fff;
          padding: 1.5rem;
          border: 1px solid #dee2e6;
          box-shadow: 0 .125rem .25rem rgba(0,0,0,.075)!important;
          h2 {
            font-size: 24px;
            font-weight: 500;
            margin-bottom: 8px;
          }
          p {
            font-size: 16px;
            display: block;
            margin-bottom: 16px !important;
            padding: 0;
          }
          span {
            font-size: 14px;
          }
          .social-media-circle {
            width: 31px;
            height: 31px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #fff;
            text-align: center;
            border: 1px solid transparent;
          }
        }
      }
    }
  }
  .have-earned {
    .box {
      border-radius: 0.3rem;
      border: 1px solid #dee2e6!important;
      box-shadow: 0 .125rem .25rem rgba(0,0,0,.075)!important;
    }
  }
}
</style>
