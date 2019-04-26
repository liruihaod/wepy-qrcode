# weapp-qrcode

微信小程序生成二维码工具 wepy组件

具体使用方法参考 `src/index/index.wpy`文件
## 使用方法

引入组件

```

import Qrcode from "../../components/qrcode"

 components = {
    qrcode:Qrcode
  };
    data = {
    text:"",
    colorLight:"",
    colorLight:"",
    width:"",
    height:"",
  };
```

使用标签

```
<qrcode
        :text.sync="text"
        :height.sync="height"
        :colorDark.sync="colorDark"
        :colorLight.sync="colorLight"
        :width.sync="width" />
```

`text`为需要转化为二维码的字符串；

`width`和`height`为绘制出的二维码长宽，默认宽高为 150；

`colorDark`和`colorLight`为二维码交替的两种颜色，默认黑白两色；

修改`text`属性自动修改二维码


