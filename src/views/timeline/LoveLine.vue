<template>
  <div class="block">
    <picture-wall></picture-wall>
    <el-timeline style="margin-left: 30%;width: 40%;margin-top: 5%">
      <el-timeline-item placement="top" v-for="(activity, index) in activities"
                        :key="index"
                        :icon="activity.icon"
                        :type="activity.type"
                        :color="activity.color"
                        :size="activity.size"
                        :timestamp="activity.timestamp">
        <div slot="dot"><img src="../../assets/kiss/kiss1.jpeg" style="width:30px;height:30px;border-radius: 15px;margin-left: -10px"></div>
        <el-card shadow="hover" style="background-color: #f7f7f7; margin-bottom: 40px">
          <h4>{{activity.content}}</h4>
          <p>{{activity.user}} 提交于 {{activity.timestamp}}</p>
        </el-card>
      </el-timeline-item>
    </el-timeline>
  </div>
</template>
<script>
  import PictureWall from './PictureWall'

  export default {
    components: {
      PictureWall
    },
    data () {
      return {
        activities: [
          {
            content: '支持使用图标',
            timestamp: '2018-04-12 20:46',
            size: 'large',
            icon: 'el-icon-apple',
            color: 'pink',
            user: 'gengleiming',
          },
          {
            content: '支持自定义颜色',
            timestamp: '2018-04-03 20:46',
            size: 'large',
            icon: 'el-icon-sugar',
            color: 'green',
            user: 'gengleiming',
          },
          {
            content: '支持自定义尺寸',
            timestamp: '2018-04-03 20:46',
            size: 'large',
            icon: 'el-icon-sugar',
            color: 'pink',
            user: 'gengleiming',
          },
          {
            content: '默认样式的节点',
            timestamp: '2018-04-03 20:46',
            size: 'large',
            icon: 'el-icon-sugar',
            color: 'pink',
            user: 'gengleiming',
          }]
      }
    }
  }
</script>
