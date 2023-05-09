# study-ARIA
> Accessible Rich Internet Applications (ARIA)

# demo
### role = tablist & role = tab

### role = none 等价 role = presentation

移除元素上隐式的ARIA语义，比如：xxx 按钮

# 遇到的问题

（react项目）在实践中，发现读2次。比如：头部有个会退按钮，设置的文案“回退”。

排查下来，是因为回退按钮是通过*TouchableOpacity*实现的，框架对*TouchableOpacity*组件做封装的时候添加了一个 tabIndex 属性，并且固定value为1导致在使用TouchableOpacity实现组件的时候都被当作一个组

# 参考文档
[roles](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles)
[eslint jsx a11y](https://github.com/evcohen/eslint-plugin-jsx-a11y)
[react native相关的accessibility](https://reactnative.dev/docs/accessibility#aria-label)
