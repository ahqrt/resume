<script setup lang="ts">
function handlePrint() {
  window.print()
}

function handleGithub() {
  window.open('https://github.com/varletjs/varlet-resume')
}
</script>

<template>
  <var-app-bar image="@/assets/23964.jpg"
    image-linear-gradient="to right top, rgba(72, 151, 221, 1) 0%, rgba(47, 0, 208, 0.1) 100%">
    <template #content>
      <div class="resume-app-bar-content">
        <div class="resume-app-bar-content-inner">
          <var-row :gutter="20">
            <var-col :span="8" :xs="24" justify="center">
              <var-avatar :size="180" bordered src="@/assets/avatar.jpg" />
            </var-col>
            <var-col direction="column" :span="16" :xs="24">
              <div class="resume-app-bar-name">杨立业</div>
              <div class="resume-app-bar-job">前端开发工程师</div>
              <div class="resume-app-bar-description">
                3年前端开发经验，对技术有热情，写代码有洁癖，能够⾼效的完成开发任务。能够搭建完善的前端⼯具链和工作流，有中大型前端项目开发经验。积极拥抱开源，有⾃⼰持续维护的开源项⽬，且有一直在学习新技术的热情并且付诸行动。
              </div>
            </var-col>
          </var-row>
        </div>
      </div>
    </template>
  </var-app-bar>
</template>

<style lang="less" scoped>
.resume-app-bar {

  &-content {
    display: flex;
    justify-content: center;
  }

  &-content-inner {
    width: 760px;
    padding: 30px 20px 70px;
  }

  &-name {
    font-size: 36px;
    margin-top: 10px;
    font-weight: bold;
  }

  &-job {
    font-size: 20px;
    margin-top: 6px;
    padding: 0 3px;
  }

  &-description {
    font-size: 15px;
    margin-top: 20px;
    color: #eee;
    line-height: 24px;
    padding: 0 3px;
  }
}
</style>
