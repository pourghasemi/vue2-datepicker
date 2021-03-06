## [2.6.3](https://github.com/mengxiong10/vue2-datepicker/compare/v2.6.2...v2.6.3) (2018-12-08)


### 修复Bug

* 修复手动输入范围时无法成功的问题 ([#209](https://github.com/mengxiong10/vue2-datepicker/issues/209)) ([97289d1](https://github.com/mengxiong10/vue2-datepicker/commit/97289d1))



## [2.6.2](https://github.com/mengxiong10/vue2-datepicker/compare/v2.6.1...v2.6.2) (2018-10-30)


### 修复Bug

* `calendar-change`事件在正确的时候触发 ([b1a5a41](https://github.com/mengxiong10/vue2-datepicker/commit/b1a5a41))


### 新功能

* 添加 `calendar-change` 事件 ([ef9314e](https://github.com/mengxiong10/vue2-datepicker/commit/ef9314e))



## [2.6.1](https://github.com/mengxiong10/vue2-datepicker/compare/v2.6.0...v2.6.1) (2018-10-17)


### 修复Bug

* 阻止组件的事件冒泡到外面 ([de177d8](https://github.com/mengxiong10/vue2-datepicker/commit/de177d8))


### 新功能

* script直接引用的时候自动注册组件 ([a310f59](https://github.com/mengxiong10/vue2-datepicker/commit/a310f59))



# [2.6.0](https://github.com/mengxiong10/vue2-datepicker/compare/v2.5.0...v2.6.0) (2018-10-11)


### 修复Bug

* 修复快捷方式的颜色 ([ac4aa87](https://github.com/mengxiong10/vue2-datepicker/commit/ac4aa87))


### 新功能

*  添加属性 `appendToBody` ([e26e1f5](https://github.com/mengxiong10/vue2-datepicker/commit/e26e1f5))


# [2.5.0](https://github.com/mengxiong10/vue2-datepicker/compare/v2.4.3...v2.5.0) (2018-10-05)

### 新功能

* 添加 `panel-change` 事件 ([5cdba7b](https://github.com/mengxiong10/vue2-datepicker/commit/5cdba7b))


## [2.4.3](https://github.com/mengxiong10/vue2-datepicker/compare/v2.4.0...v2.4.3) (2018-09-28)

### 修复Bug

* 修复选择时间时候显示'am', 'pm' ([8e475b3](https://github.com/mengxiong10/vue2-datepicker/commit/8e475b3))
* 修复一个IE兼容性问题 ([fefed17](https://github.com/mengxiong10/vue2-datepicker/commit/fefed17))
* 当选择一个时间的时候关闭面板 ([#154](https://github.com/mengxiong10/vue2-datepicker/issues/154)) ([12907ad](https://github.com/mengxiong10/vue2-datepicker/commit/12907ad))
* 修复年和月的禁用函数错误 ([#169](https://github.com/mengxiong10/vue2-datepicker/issues/169)) ([42bc068](https://github.com/mengxiong10/vue2-datepicker/commit/42bc068))

### 新功能

*  添加一个`clear`事件 ([e0776b6](https://github.com/mengxiong10/vue2-datepicker/commit/e0776b6))


<a name="2.4.0"></a>
# [2.4.0](https://github.com/mengxiong10/vue2-datepicker/compare/v2.3.2...v2.4.0) (2018-08-08)


### 新功能

* 添加属性`type`为`time`的时候只显示时间组件

## [2.3.2](https://github.com/mengxiong10/vue2-datepicker/compare/v2.2.0...v2.3.2) (2018-08-07)

### 新功能

* 添加属性 `date-format` 格式化时间组件头部和日期的tooltip

# [2.2.0](https://github.com/mengxiong10/vue2-datepicker/compare/v2.1.0...v2.2.0) (2018-08-06)

### 修复bug

* 设置input的autocomplete为off避免下拉框的干扰

### 新功能

* 添加时间'change-calendar-yeaer', 'change-calendar-month'方便联动两个窗口


# [2.1.0]() (2018-07-24)


### 新功能

* 添加`type` 支持月和年的单独选择


# [2.0.0]() (2018-06-16)

### 新功能

* 添加`clearable` 用于控制是否显示清除按钮
* 添加 slot `calendar-icon` 自定义日历图标
* 添加 slot `header` 和 `footer` 自定义弹出日历的头部和尾部
* `disabledDays` 现在支持函数

### 非兼容性更新

* 重构代码. 如果你自己hack过代码可能会失效
* `format` 默认值由 yyyy-MM-dd 改成 YYYY-MM-DD, 现在格式类似moment.js. 不支持小写的yyyy
* 移除了`custom-formatter`
* `editable` 默认由false改成true, 现在日历范围也支持手动修改
* 当选择年或月的面板的时候不会修改日期(因为当设置了`not-before`或者`not-after`的时候会引发很多问题和bug)
