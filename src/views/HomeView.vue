<template>
  <!-- <v-container>
    <v-row>
      <v-col class="md-6 " v-for="(item,index) in list" :key="index">

        <web-site
        :url="item.url"
        :logoImg="item.logoImg"
        :title="item.title"
        :subTitle="item.subtitle"
        >

        </web-site>
      </v-col>
    </v-row>
     <v-row>
      <v-col class="md-6 " v-for="(item,index) in list" :key="index">

        <web-site
        :url="item.url"
        :logoImg="item.logoImg"
        :title="item.title"
        :subTitle="item.subtitle"
        >

        </web-site>
      </v-col>
    </v-row>
     <v-row>
      <v-col class="md-6 " v-for="(item,index) in list" :key="index">

        <web-site
        :url="item.url"
        :logoImg="item.logoImg"
        :title="item.title"
        :subTitle="item.subtitle"
        >

        </web-site>
      </v-col>
    </v-row>
     <v-row>
      <v-col class="md-6 " v-for="(item,index) in list" :key="index">

        <web-site
        :url="item.url"
        :logoImg="item.logoImg"
        :title="item.title"
        :subTitle="item.subtitle"
        >

        </web-site>
      </v-col>
    </v-row>
  </v-container> -->
   <v-carousel v-model="model">
    <v-carousel-item
      v-for="(color, i) in colors"
      :key="color"
    >
      <v-sheet
        :color="color"
        height="100%"
        tile
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <div class="text-h2">
            Slide {{ i + 1 }}
          </div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
import WebSite from '@/components/WebSite.vue'


  export default {
    name: 'Home',

    components: {
      WebSite,
    },
    data:() => ({
      model: 0,
      colors: [
        'primary',
        'secondary',
        'yellow darken-2',
        'red',
        'orange',
      ],
    }),
    
//     data(){
//       return {
//           list: [
//             {
//           url: 'https://www.aliyun.com/"',
//           logoImg: "http://47.96.31.161:9000/my-file/icon/aliyun.png",
//           title: "阿里云",
//           subtitle: "点击领取200元阿里云优惠券",
//         }, 

// {
//           url: 'https://www.aliyun.com/"',
//           logoImg: "http://47.96.31.161:9000/my-file/icon/tengxunyun.png",
//           title: "腾讯云",
//           subtitle: "点击领取200元腾讯云优惠券",
//         },
//         {
//           url: 'https://www.aliyun.com/"',
//           logoImg: "http://47.96.31.161:9000/my-file/icon/huaweiyun.png",
//           title: "华为云",
//           subtitle: "点击领取200元华为云优惠券",
//         },
//         {
//           url: 'https://www.aliyun.com/"',
//           logoImg: "http://47.96.31.161:9000/my-file/icon/qiniuyun.png",
//           title: "七牛云",
//           subtitle: "点击领取200元华为云优惠券",
//         }, 

//           ]
//       }
    // }
  }
</script>
