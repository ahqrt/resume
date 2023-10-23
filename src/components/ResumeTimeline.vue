<script setup lang="ts">
import { ref } from 'vue'

const companies = ref([
  {
    label: '百家云集团有限公司',
    date: '2021/09-至今',
    description: '任前端技术leader，主要负责视频会议web端和pc端的saas sdk开发。',
  },
  {
    label: '山东兆物网络技术股份有限公司',
    date: '2020/03-2021/08',
    description: '任初级前端开发工程师，主要负责还原设计图，混合开发应用的编写和打包。',
  },
])
</script>

<template>
  <resume-block title="工作经历">
    <var-steps class="resume-timeline" direction="vertical" :active="companies.length - 1">
      <var-step current-icon="map-marker" active-icon="map-marker" v-for="c in companies" :key="c.label">
        <div class="resume-timeline-company">
          <div class="resume-timeline-label">{{ c.label }}</div>
          <div class="resume-timeline-date">{{ c.date }}</div>
          <div class="resume-timeline-description">{{ c.description }}</div>
        </div>
      </var-step>
    </var-steps>
  </resume-block>
</template>

<style lang="less" scoped>
.resume-timeline {
  &-company {
    margin-left: 10px;
  }

  &-label {
    font-size: 16px;
  }

  &-date {
    color: #aaa;
    margin: 6px 0;
  }

  &-description {
    color: #555;
  }
}
</style>
