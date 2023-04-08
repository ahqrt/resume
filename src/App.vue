<template>
  <resume-app-bar />

  <div class="resume-layout">
    <resume-profile />

    <resume-blank :size="350"></resume-blank>

    <var-row :gutter="20">
      <var-col :span="24" :xs="24">
        <resume-timeline />
      </var-col>
      <!-- <var-col :span="12" :xs="24">
        <resume-skills />
      </var-col> -->
    </var-row>

    <resume-blank :size="350"></resume-blank>

    <resume-block title="项目经历" subtitle="**只列举部分典型项目**">
      <resume-block-item title="boom视频会议"
        description="基于WebRTC的视频会议系统，主要技术栈是Typescript，React，Electron，React Native，在产品中主要负责会议内底层saas sdk的开发维护，主要开发会议内推拉流相关的业务模型开发维护，以及端上JsonRPC信令系统的开发和维护，提升大型会议系统的稳定性和性能。" />
      <resume-block-item title="中债一体化学习平台"
        description="该项目是为了满足中债公司内部业务需求而开发的学习平台，主要是做内部视频会议学习，考试系统。主要技术栈是React，React Native，React Native Web。在项目中主要负责使用React Native， React Native Web搭建开发一套代码三端运行的敏捷开发模式，和主要的视频会议和考试视频监控功能。" />
      <resume-block-item title="烟草舆情分析系统"
        description="该项目是为了满足烟草局业务需求开发的分析系统，主要是基于舆情数据做可视化展示、可视化分析。主要技术栈是Vue2全家桶 + Echarts + AntV G2，在项目中主要负责做可视化展示部分，包括各种数据大屏，以及可视化分析模块。" />
    </resume-block>

    <resume-block title="开源项目">
      <resume-block-item title="varletjs/varlet (核心开发者)"
        description="一个基于 Vue3 的 Material Design 风格移动端组件库，尤雨溪 Vue 官方团队 2021 年 Vue Conf 推荐、Gitee GVP 年度最有价值开源项目、阮一峰周刊推荐。提供 60+ 个高质量通用组件，支持按需引入，国际化、SSR、暗黑模式、90% 以上的单元测试覆盖率，并提供了 VSCode 插件。" />
    </resume-block>

    <resume-block title="技能清单">
      <resume-block-compact-item description="熟悉WebRTC和web音视频开发相关技术" />
      <resume-block-compact-item description="熟练使⽤ html5、css3、JavaScript、Typescript 构建 web 应⽤" />
      <resume-block-compact-item description="熟练使用 Vue、React 及其生态系统" />
      <resume-block-compact-item description="熟练使用 Vite、Rollup、Webpack，能完成定制化插件的编写" />
      <resume-block-compact-item description="熟练使用 Jest、Vitest 等单元测试工具" />
      <resume-block-compact-item description="熟练使用 eslint、stylelint、prettier、husky、lint-staged、commitlint 等工具进行代码规范约束" />
      <resume-block-compact-item description="熟练使用 git、svn 版本控制软件" />
      <resume-block-compact-item description="熟练使用 react-native、electron 跨端开发" />
      <resume-block-compact-item description="学习过 Rust、C++ 并有一定的理解和实际编码经验" />
    </resume-block>
  </div>
</template>

<style>
* {
  box-sizing: border-box;
}

@media print {
  * {
    box-shadow: none !important;
  }

  .print-disabled {
    display: none !important;
  }
}

body {
  margin: 0;
  font-family: 'Roboto', sans-serif;
  transition: background-color 0.25s, color 0.25s;
  color: var(--color-text);
  background-color: var(--color-body);
}

::-webkit-scrollbar {
  display: none;
}
</style>

<style lang="less" scoped>
.resume-layout {
  padding: 0 20px 30px;
}
</style>
