<template>
  <vs-row>
    <vs-col :key="i"  v-for="(tr, i) in offers"
             :data="tr" class="cardColum" type="flex" vs-justify="centerr" vs-align="space-around" vs-w="4" vs-sm="12">
      <vs-card actionable class="cardx">
        <div slot="header">
          <vs-row vs-type="flex" vs-justify="space-between">
            <vs-col vs-justify="flex-start" vs-align="flex-start">
              <h3>
                {{tr.name}}
              </h3>
            </vs-col>
            <vs-col vs-offset="8">
              <div class="con-avatar-solo">
                <vs-avatar src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTQ6O0aXz-lOZreE476UiwZv_fMY3ZG30TCLMpNPzIZsvTp2St_&usqp=CAU" />
                <vs-avatar type="gradient" color="success" badge="152" icon="whatshot" />
                <vs-avatar type="gradient" color="warning" badge="35" icon="share" />
              </div>
            </vs-col>
          </vs-row>
<!--          <h3>
            {{tr.name}}
          </h3>
          <div class="con-avatar-solo">
            <vs-avatar src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTQ6O0aXz-lOZreE476UiwZv_fMY3ZG30TCLMpNPzIZsvTp2St_&usqp=CAU" />
            <vs-avatar type="gradient" color="success" badge="152" icon="whatshot" />
            <vs-avatar type="gradient" color="warning" badge="35" icon="share" />
          </div>-->
        </div>
        <div slot="media">
          <img :src="tr.urlImg">
        </div>
        <div>
          <span> {{tr.description}}</span>
        </div>
        <div slot="footer">
          <vs-row vs-justify="flex-end">
            <vs-button class="buttonCard" badge="2" type="gradient" color="danger" icon="favorite"></vs-button>
            <vs-button class="buttonCard" type="gradient" color="primary" icon="turned_in_not"></vs-button>
            <vs-button class="buttonCard" type="gradient" color="success" icon="link"></vs-button>
          </vs-row>
        </div>
      </vs-card>
    </vs-col>
  </vs-row>
</template>

<script>
export default {
  name: 'CardItem',
  data: () => ({
    offers: [
      {
        id: 1,
        name: 'Televisor Sony 42 Pulgadas',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        refLink: 'www.google.com',
        website: 'hildegard.org',
        urlImg: 'https://www.worten.es/i/88054848102294abd0b46dd9a9b0270e0b71d3b7.jpg'
      },
      {
        id: 2,
        name: 'Televisor Sony 42 Pulgadas',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        refLink: 'www.google.com',
        website: 'hildegard.org',
        urlImg: 'https://www.worten.es/i/88054848102294abd0b46dd9a9b0270e0b71d3b7.jpg'
      },
      {
        id: 3,
        name: 'Televisor Sony 42 Pulgadas',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        refLink: 'www.google.com',
        website: 'hildegard.org',
        urlImg: 'https://www.worten.es/i/88054848102294abd0b46dd9a9b0270e0b71d3b7.jpg'
      },
      {
        id: 4,
        name: 'Televisor Sony 42 Pulgadas',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        refLink: 'www.google.com',
        website: 'hildegard.org',
        urlImg: 'https://www.worten.es/i/88054848102294abd0b46dd9a9b0270e0b71d3b7.jpg'
      },
      {
        id: 5,
        name: 'Televisor Sony 42 Pulgadas',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        refLink: 'www.google.com',
        website: 'hildegard.org',
        urlImg: 'https://www.worten.es/i/88054848102294abd0b46dd9a9b0270e0b71d3b7.jpg'
      },
      {
        id: 6,
        name: 'Televisor Sony 42 Pulgadas',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        refLink: 'www.google.com',
        website: 'hildegard.org',
        urlImg: 'https://www.worten.es/i/88054848102294abd0b46dd9a9b0270e0b71d3b7.jpg'
      },
      {
        id: 7,
        name: 'Televisor Sony 42 Pulgadas',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        refLink: 'www.google.com',
        website: 'hildegard.org',
        urlImg: 'https://www.worten.es/i/88054848102294abd0b46dd9a9b0270e0b71d3b7.jpg'
      },
      {
        id: 8,
        name: 'Televisor Sony 42 Pulgadas',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        refLink: 'www.google.com',
        website: 'hildegard.org',
        urlImg: 'https://www.worten.es/i/88054848102294abd0b46dd9a9b0270e0b71d3b7.jpg'
      },
      {
        id: 9,
        name: 'Televisor Sony 42 Pulgadas',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        refLink: 'www.google.com',
        website: 'hildegard.org',
        urlImg: 'https://www.worten.es/i/88054848102294abd0b46dd9a9b0270e0b71d3b7.jpg'
      },
      {
        id: 10,
        name: 'Televisor Sony 42 Pulgadas',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        refLink: 'www.google.com',
        website: 'hildegard.org',
        urlImg: 'https://www.worten.es/i/88054848102294abd0b46dd9a9b0270e0b71d3b7.jpg'
      }
    ]
  })
}
</script>

<style scoped>
  .cardColum,.buttonCard{
    padding-left: 1em;
    padding-right: 1em;

  }
  .cardx{
    margin: 16px 0;
    box-shadow: 1px 1px 5px #505050, 0px 0px 0px #E6E6E6, 0px 0px 0px #505050;
    border-radius: 4px;
  }
</style>
