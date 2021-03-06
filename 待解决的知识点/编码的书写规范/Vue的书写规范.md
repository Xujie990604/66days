# Vue中的书写和命名格式

## 命名格式

### 组件名

* 在DOM里面使用一个组件的时候。字母全部小写并且必须包含一个连字符，组件名必须是多单词的。这会帮助你避免和现在的和未来的HTML元素相冲突
* 组件名推荐全部小写用横线连接,并且组件名定义时可以用MyComponent来定义，调用时使用my-component来调用
* 组件文件名字大驼峰命名

* 和父组件紧密耦合的子组件的名字要使用父组件名作为开头  父组件 Home 子组件 HomeNav HomeFooter
* 相同类型的组件有相同的前缀。

### prop

* 在组件中进行传值的时候使用kebab-case(小写字母，中划线的版本)形式
* 在组件接收值的时候，使用小驼峰形式。

## 事件

* 事件不同于组件和prop，不存在任何的自动化大小写转换。推荐始终使用 kebab-case 的事件名

## 书写格式

### 缩进两个空格是标准

## v-for

* 使用v-for的时候必须配合key来使用
* v-for和v-if不作用于同一个DOM上

## v-if

* 如果一组v-if或者v-else的元素类型相同，如果不加入key的话，很可能会在切换的时候直接复用DOM。

## 尽量使用Vuex来管理数据。而不是使用事件总线

### css

* css的类名使用kebab-case(小写字母，中划线的版本)