# 快速开始

## 安装

```
# yarn install
yarn add @pansy/react-watermark

# npm install
npm install --save @pansy/react-watermark
```

## 使用

```
import React from 'react';
import Watermark from '@pansy/react-watermark';

export default () => {
  return (
    <WaterMark style={{ width: 500, height: '100%' }} text="测试水印">
      <div>
        <button>
          123
        </button>
      </div>
    </WaterMark>
  )
}
```

## API

| 参数          | 说明          | 类型                 | 默认值 | 版本 |
| ------------ | --------------| ------------------- | ------ | ---- |
| style        | 额外的样式      | `CSSProperties`     | --     | --   |
| zIndex        | 水印层级      | `number`     | `9999`     | 1.0.2   |
| monitor      | 监听水印元素是否被篡改，被修改或者删除等操作，则重新渲染水印 | `boolean`           | `true` | --   |
| text         | 水印文本        | `string`            |  --   | --   |
| options      | 水印配置        | `object`            | `{...}`    | --   |

**options**

| 参数          | 说明          | 类型                 | 默认值 | 版本 |
| ------------ | --------------| ------------------- | ------ | ---- |
| width        | 单个水印区域宽度  | `number`           | `160`    | --   |
| height      | 单个水印区域高度   | `number`           | `80` | --   |
| opacity      | 透明度          | `number`           |  `0.2`   | --   |
| rotate      | 旋转的角度        | `number`           | `20`     | --   |
| fontSize      | 字体大小          | `number`           |  `14`   | --   |
| fontWeight    | 字体粗细        | --           | `normal`   | --   |
| fontColor      | 字体颜色        | `string`      |  `#727071`   | --   |
| fontFamily    | 规定字体系列      | `string`      | `sans-serif`    | --   |
