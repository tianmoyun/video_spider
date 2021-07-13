![video_spider](https://socialify.git.ci/5ime/video_spider/image?description=1&descriptionEditable=%E6%94%AF%E6%8C%8117%E4%B8%AA%E7%9F%AD%E8%A7%86%E9%A2%91%E5%B9%B3%E5%8F%B0%E5%8E%BB%E6%B0%B4%E5%8D%B0%E4%B8%8B%E8%BD%BD&font=Inter&forks=1&language=1&owner=1&pattern=Circuit%20Board&stargazers=1&theme=Light)

目前支持21个平台视频去水印下载，欢迎各位Star，**提交issues时请附带视频链接**。

## 支持平台

| 平台 | 状态| 平台 | 状态| 平台 | 状态| 平台 | 状态| 平台 | 状态|
|  ----  | ----  | ----  | ---- |----|----|----|----|----|----|
| 皮皮虾 | ✔ | 抖音短视频 | ✔ | 火山短视频 | ✔| 皮皮搞笑 | ✔ | 全民K歌 | ✔ |
| 微视短视频 | ✔ | 微博 | ✔ | 最右 | ✔| vuevlog | ✔ |小咖秀| ✔|
| 轻视频 | ✔ | 快手短视频 | ✔ | 全民小视频 | ✔|陌陌 | ✔ | Before避风 | ✔ |
| 西瓜视频 | ✔|逗拍|✔|虎牙|✔|6间房|✔|梨视频|✔|
| 新片场 | ✔|||||||||

## 请求示例

支持GET/POST `url`参数必填

## 返回数据

| 字段名 | 说明 | 字段名 | 说明 |字段名 | 说明 |字段名 | 说明 |
|  ----  | ----  | ----  | ---- |---- |---- |----|----|
| author | 视频作者| avatar | 作者头像 | like | 视频点赞量 | time | 视频发布时间 |
| title | 视频标题 | cover | 视频封面 | url | 视频无水印链接 | sex  | 作者性别 |
| age | 作者年龄 | city | 所在城市 | uid | 作者id | code | 状态码 |


## 调用示例

如果你不会调用 我在`demo`目录下放两个最基本的调用演示

- `demo.html`第`98`行请修改为`你的接口地址`
- `demo.py`第`7`行请修改为`你的接口地址`

## 更新日志

- 2021/2/21 新增微视 isee前缀域名，新增皮皮搞笑 修复微博匹配失败
- 2021/2/23 修复全民匹配失败，修复避风匹配失败，新增全民K歌
- 2021/3/26 新增视频解析失败返回`201`参数
- 2021/3/27 新增西瓜视频 <s>请在`video_spider.php`文件第`426`行填写你的西瓜视频`cookies`,无需登录</s>
- 2021/4/26 新增皮皮搞笑`pipigx`主域
- 2021/6/22 修复抖音解析失败
- 2021/7/6 修复皮皮虾解析失败
- 2021/7/7 修复最右，西瓜视频，微博，感谢 @yzh52521 提供代码
- 2021/7/8 修复西瓜视频，新增逗拍，感谢 @yzh52521 提供代码
- 2021/7/12 新增虎牙/6间房/梨视频
- 2021/7/13 新增新片场视频
## FAQ

**为什么演示网址界面和`demo`文件夹里的不一样**

因为我用vue重写了(https://github.com/5ime/vue-page)

**网址中包含特殊字符导致GET请求无法传递正确的参数值**

传递的参数中包含`#&=`之类的，可能无法正确传递参数值，建议使用`POST请求`或`urlencode编码`后进行GET请求

## 免责声明

本仓库只为学习研究，如涉及侵犯个人或者团体利益，请与我取得联系，我将主动删除一切相关资料，谢谢！
