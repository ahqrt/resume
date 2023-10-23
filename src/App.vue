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

    <resume-block title="项目经历" subtitle="只列举部分典型项目">
      <resume-block-item title="boom视频会议">
        <p>项目简介: 基于WebRTC的视频会议系统</p>
        <p>技术栈: Typescript，React，Electron，React Native</p>
        <p>工作内容：</p>
        <p>1. 在系统早期版本主要负责功能迭代和维护。</p>
        <p>2. 后续在会议2.0升级中，作为前端技术leader，和架构师确定web和pc整体会议系统的升级迭代技术选型。</p>
        <p>3. 独立负责会议sdk核心底层功能，主要包括会议内推拉流相关的业务模型，以及端上JsonRPC信令系统的开发和维护。
          设计并实现了一个基于状态机的异步任务管理系统，解决了会议系统中异步任务时序混乱的问题，提升了会议系统的稳定性。
        </p>
        <p>4. 设计端上应用层的整体拆分，以应对不同的项目和产品需求，将视频会议应用拆分成不同的子单元，根据需求自由组合产品形式，实现模块化开发功能。</p>
        <p>5. 万人视频会议功能开发中，重新设计整体的会议业务模型，设计了从依赖流状态到业务状态的转换，解决了会议系统中存储流信息消耗内存过大的问题，
          简化了状态的同步逻辑，提升了会议系统的流畅度。实现了从最早版本200人不稳定的视频会议应用，到现在支持上万人同时在线的稳定视频会议应用。</p>
        <p>6. 在万人视频会议功能开发中，处理排查过比较复杂的内存泄漏问题。解决因为内存溢出导致的客户端崩溃问题。</p>
        <p>7. pc客户端主要通过electron开发，在实际的功能开发中，通过node addon的方式，实现了electron和c++的交互，实现了共享本地声音，共享播放ppt等webrtc原生不支持的功能。
          提升了pc客户端的性能，扩展了pc客户端的功能。</p>
      </resume-block-item>
      <resume-block-item title="boom-engineering-kit">
        <p>项目简介: 部门前端组基础工具包</p>
        <p>技术栈: Typescript，React，React Native, Electron</p>
        <p>工作内容：</p>
        <p>1. 开发的前端部门的cli工具，包括各种开发环境的template 脚手架，以及各种开发工具的插件，包括eslint，stylelint，prettier，husky，lint-staged，commitlint等。
        </p>
        <p>2. 会议应用的公共组件，包括播放器，视频会议组件，以及各种业务组件。</p>
        <p>3. 会议应用的公共工具库，包括各种工具函数，以及各种业务工具函数。</p>
        <p>4. Electron 中 IPC 通信相关的逻辑功能拆分，封装成单独的electron sdk，方便客户和第三方项目集成。</p>
        <p>5. cpp addon 插件 sdk封装，方便第三方项目和客户集成。</p>
      </resume-block-item>
      <resume-block-item title="中债一体化学习平台">
        <p>项目简介: 基于视频会议应用的产品化项目开发</p>
        <p>技术栈: React，React Native, React Native Web</p>
        <p>工作内容：</p>
        <p>1. 在项目中主要负责使用 React Native，React Native Web搭建开发一套代码在web， iOS，Android都可以运行的敏捷开发架构模式。</p>
        <p>2. 负责前期项目的搭建，包括移动端和web端的路由拆分，通用组件的开发，以及响应式布局。</p>
        <p>3. 主要的视频会议和考试视频监控功能。</p>
      </resume-block-item>
    </resume-block>

    <resume-block title="开源项目">
      <resume-block-item title="varletjs/varlet (核心开发者)">
        <p>一个基于 Vue3 的 Material Design 风格移动端组件库，尤雨溪 Vue 官方团队 2021 年 Vue Conf 推荐、Gitee GVP 年度最有价值开源项目、阮一峰周刊推荐。提供 60+
          个高质量通用组件，支持按需引入，国际化、SSR、暗黑模式、90% 以上的单元测试覆盖率，并提供了 VSCode 插件。</p>
      </resume-block-item>
      <resume-block-item title="mdn/webaudio-example">
        <p>MDN web audio article 系列部分章节内容输出，文档错误校验。</p>
      </resume-block-item>
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
