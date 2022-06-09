:: BASE_DOC ::

## API
### Tabs Props

名称 | 类型 | 默认值 | 说明 | 必传
-- | -- | -- | -- | --
className | String | - | 类名 | N
style | Object | - | 样式，TS 类型：`React.CSSProperties` | N
addable | Boolean | false | 选项卡是否可增加 | N
disabled | Boolean | false | 是否禁用选项卡 | N
list | Array | - | 选项卡列表。TS 类型：`Array<TdTabPanelProps>` | N
placement | String | top | 选项卡位置。可选项：left/top/bottom/right | N
size | String | medium | 组件尺寸。可选项：medium/large | N
theme | String | normal | 选项卡风格，包含 默认风格 和 卡片风格两种。可选项：normal/card | N
value | String / Number | - | 激活的选项卡值。TS 类型：`TabValue` `type TabValue = string | number`。[详细类型定义](https://github.com/Tencent/tdesign-react/blob/develop/src/tabs/type.ts) | N
defaultValue | String / Number | - | 激活的选项卡值。非受控属性。TS 类型：`TabValue` `type TabValue = string | number`。[详细类型定义](https://github.com/Tencent/tdesign-react/blob/develop/src/tabs/type.ts) | N
onAdd | Function |  | TS 类型：`(context: { e: MouseEvent }) => void`<br/>添加选项卡时触发 | N
onChange | Function |  | TS 类型：`(value: TabValue) => void`<br/>激活的选项卡发生变化时触发 | N
onRemove | Function |  | TS 类型：`(options: { value: TabValue; index: number; e: MouseEvent }) => void`<br/>删除选项卡时触发 | N

### TabPanel Props

名称 | 类型 | 默认值 | 说明 | 必传
-- | -- | -- | -- | --
className | String | - | 类名 | N
style | Object | - | 样式，TS 类型：`React.CSSProperties` | N
destroyOnHide | Boolean | true | 选项卡内容隐藏时是否销毁 | N
disabled | Boolean | false | 是否禁用当前选项卡 | N
label | TNode | - | 选项卡名称，可自定义选项卡导航内容。TS 类型：`string | TNode`。[通用类型定义](https://github.com/Tencent/tdesign-react/blob/develop/src/common.ts) | N
panel | TNode | - | 用于自定义选项卡面板内容。TS 类型：`string | TNode`。[通用类型定义](https://github.com/Tencent/tdesign-react/blob/develop/src/common.ts) | N
removable | Boolean | false | 当前选项卡是否允许移除 | N
value | String / Number | - | 选项卡的值，唯一标识。TS 类型：`TabValue` | N
onRemove | Function |  | TS 类型：`(options: { value: TabValue; e: MouseEvent }) => void`<br/>点击删除按钮时触发 | N