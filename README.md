# vue-web-template
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

这个模板应该帮助您开始在Vite中使用Vue 3进行开发。

## 推荐的IDE设置

为了获得最佳的开发体验，我们推荐以下IDE配置以及插件：

- [VSCode](https://code.visualstudio.com/)：强大的编辑器支持调试、Git控制、语法高亮等。
- [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar)：为Vue提供高效的语言支持。安装后请禁用Vetur。
- [TypeScript Vue 插件 (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin)：为`.vue`文件提供TypeScript支持。
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)：提供代码质量和风格的检查，帮助你遵守一致的编码规范。
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)：一个代码格式化工具，支持多种语言，确保代码风格一致性。
- [Stylelint](https://marketplace.visualstudio.com/items?itemName=stylelint.vscode-stylelint)：为CSS/SCSS/Less等样式表提供强大的风格检查。

请按照上述链接安装和配置插件，以确保你的开发环境设置正确。

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## 在 `.vue` 中进行 TypeScript 类型支持

TypeScript 默认无法处理 `.vue` 导入的类型信息，因此我们用 `vue-tsc` 替换了 `tsc` 命令行工具来进行类型检查。在编辑器中，我们需要 [TypeScript Vue 插件 (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin) 使 TypeScript 语言服务识别 `.vue` 文件的类型。

如果你感觉独立的 TypeScript 插件不够快，Volar 还实现了一个性能更好的[接管模式 (Take Over Mode)](https://github.com/johnsoncodehk/volar/discussions/471#discussioncomment-1361669)。你可以按照以下步骤启用它：

1. 禁用内置的 TypeScript 扩展
    1) 从 VSCode 的命令面板运行 `Extensions: Show Built-in Extensions`
    2) 找到 `TypeScript and JavaScript Language Features`，右键选择 `Disable (Workspace)`
2. 通过命令面板运行 `Developer: Reload Window` 重新加载 VSCode 窗口。


## 自定义配置

参见 [Vite 配置参考](https://vitejs.dev/config/)。

## 项目启动

### node版本
v20.9.0+

### 包管理器 

npm

<!-- ### package.json scripts 介绍 -->
## 脚本说明

在项目中，我们通过在 `package.json` 中定义了一系列的脚本来执行常见的任务，以下是每个脚本的详细说明：

- `npm run dev`: 启动Vite开发服务器，开启本地开发环境，支持热重载。
- `npm run build`: 先进行类型检查，然后构建生产环境下的应用。它会运行 `type-check` 和 `build-only` 脚本。
- `npm run preview`: 本地预览生产构建的项目。
- `npm run test:unit`: 运行Vitest进行单元测试。
- `npm run test:run`: 使用Vitest执行测试并直接在控制台显示结果。
- `npm run build-only`: 单独执行Vite构建流程，为生产环境编译和压缩代码。
- `npm run type-check`: 使用 `vue-tsc` 对项目中的TypeScript类型进行检查，但不生成代码。
- `npm run lint`: 运行ESLint进行代码风格检查和修复，它会检查`.vue`、`.js`、`.jsx`、`.cjs`、`.mjs`、`.ts`、`.tsx`、`.cts`、`.mts`文件。
- `npm run format`: 运行Prettier格式化`src/`目录下的代码，以保证代码风格的一致性。
- `npm run cm`: 运行`cz`，为提交信息提供更易读的提交规范。
- `npm run prepare`: 运行`husky install`，设置Git钩子。
- `npm run lint:style`: 运行Stylelint进行样式文件的风格检查和修复，它会检查所有`.css`和`.vue`文件。

确保在提交代码前运行相应的脚本，以保持代码质量和风格一致性。




