<template>
  <div class="resume-profile">
    <var-row :gutter="20">
      <var-col justify="center" :span="12" :xs="24">
        <var-paper class="resume-profile-paper" :elevation="2" :radius="4">
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-cake class="resume-profile-icon" />
              <span>出生日期: 1998年02月</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-school class="resume-profile-icon" />
              <span>学校: 山东理工大学</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-calendar class="resume-profile-icon" />
              <span>工作年限: 3年</span>
            </div>
          </var-cell>

        </var-paper>
      </var-col>

      <var-col :span="12" :xs="24">
        <var-paper class="resume-profile-paper" :elevation="2" :radius="4">
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-phone class="resume-profile-icon" />
              <span>手机: 18053180656</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-email class="resume-profile-icon" />
              <span>邮箱: a18053180656@gmail.com</span>
            </div>
          </var-cell>

          <var-cell :border-offset="0">
            <div class="resume-profile-cell">
              <icon-github class="resume-profile-icon" />
              <span>Github: <a href="https://github.com/ahqrt">https://github.com/ahqrt</a></span>
            </div>
          </var-cell>
        </var-paper>
      </var-col>
    </var-row>
  </div>
</template>

<style lang="less" scoped>
.resume-profile {
  width: 100%;

  &-paper {
    width: 100%;
    margin-top: 30px;
  }

  &-cell {
    display: flex;
    align-items: center;
  }

  &-icon {
    width: 22px;
    margin-right: 10px;
    fill: var(--color-primary)
  }
}
</style>
