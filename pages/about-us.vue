<template>
    <div class="about-us">
        <PagesHero title="About Us" />
        <v-container>
            <div class="page-content pt-6 pb-10 mt-16">
                <div v-for="text in 4" :key="text" class="text">
                    <h3>What is Lorem Ipsum?</h3>
                    <p>
                        Lorem Ipsum Is Simply Dummy Text Of The Printing And Typesetting Industry. Lorem Ipsum Has Been The Industry's Standard Dummy Text Ever Since The 1500S, When An Unknown Printer Took A Galley Of Type And Scrambled It To Make A Type Specimen Book. It Has Survived Not Only Five Centuries, But Also The Leap Into Electronic Typesetting, Remaining Essentially Unchanged. It Was Popularised In The 1960S With The Release Of Letraset Sheets Containing Lorem Ipsum Passages, And More Recently With Desktop Publishing Software Like Aldus Pagemaker Including Versions Of Lorem Ipsum.
                    </p>
                </div>
                <div class="copy-right">
                    <h3>
                        All rights reserved to <a target="_blank" href="https://akwade.com">Akawde's</a> company for design and development.
                    </h3>
                  <p>
                    We, As <a target="_blank" href="https://akwade.com">Akawde's</a> Team, Are Glad To Present Our Special Package Of Any Services Or Solutions That You Might Need In The Information Technology (IT) Department. Furthermore, Our Team Is Always Ready To Provide Professional Consulting Services In Various Fields.
                  </p>
                </div>
            </div>
        </v-container>
    </div>
</template>

<style lang="scss" scoped>
.about-us {
  .page-content {
    .text {
      margin-bottom: 30px;
      h3 {
        font-size: 18px;
        font-weight: 500;
        margin-bottom: 12px;
      }
      p {
        font-weight: 400;
        font-size: 14px;
      }
    }
    .copy-right {
      box-shadow: 0 .06rem .25rem rgba(0,0,0,.17);
      padding: 28px;
      h3 {
        font-weight: 500;
        font-size: 20px;
        margin-bottom: 16px;
      }
      p {
        font-size: 16px;
        font-weight: 400;
      }
    }
  }
}
</style>
