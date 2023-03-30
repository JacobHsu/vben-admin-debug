## Vue:xhr.upload.addEventListener is not a function

项目中写上传图片功能时点击上传报此错误

vue-cli 中的 mockjs 模块把 XMLHttpRequest 覆盖拦截了，会导致对象属性访问不到，所以把 mokejs 卸载删除，删除 mokejs：

.env.production

```sh
# Whether to open mock
VITE_USE_MOCK = false # true
```
