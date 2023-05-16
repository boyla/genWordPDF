
# 如何配置模板

1. 主页点击蓝色"配置模版"链接，即可跳转配置页面，用于增删改章节模版，右侧填完提交，再点上方  保存配置，就会把所有配置保存到本地

2. 回到 施工组织设计生成 页面并刷新，就能看到最新的配置了

3. 在模版中插入特定的的花括号{}包裹的内容可以插入图片和一些模版参数，下面分别是插入方法

# 如何在模版中插入图片

1. 在要插入图片的地方，另起一行，输入模版：
   {"pdfImgName":"图片名称","width":图片宽度,"height":图片高度,"src":"图片base64编码"}

2. 把中文处依次替换成图片真实的值， 其中，图片base64编码需要把图片上传到转换网站生成，例如下边这个网站：
   http://www.ab173.com/gongju/ui/image2base64.php

完整示例：
{"pdfImgName":"施工流程图1","width":40,"height":40,"src":"data:image/gif;base64,R0lGODlhEAAQAMQAAORHHOVSKudfOulrSOp3WOyDZu6QdvCchPGolfO0o/XBs/fNwfjZ0frl3/zy7////wAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACH5BAkAABAALAAAAAAQABAAAAVVICSOZGlCQAosJ6mu7fiyZeKqNKToQGDsM8hBADgUXoGAiqhSvp5QAnQKGIgUhwFUYLCVDFCrKUE1lBavAViFIDlTImbKC5Gm2hB0SlBCBMQiB0UjIQA7"}

# 如何插入模版参数

1. 在配置模版中插入特定的双花括号包裹的字符，在生成的pdf中，这些模版会被替换顶部配置的参数，现有配置：
{{name}} 项目名称
{{address}} 项目地址
{{start_date}} 开工时间
{{end_date}} 截止时间
{{duration}} 工期
2. 一二三级标题分别用{#一级标题}，{##二级标题}，{###三级标题}配置

# 字体大小

1. 章节标题 18, 正文 10，插图标题 8
2. 一二三级标题分别为 16 14 12