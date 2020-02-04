# LAnn标注工具

## LAnn简介
![演示视频](https://freeshman.github.io/LAnn/LittleAnn.html)
LAnn（Little Annotator）是一个可以于命名实体、关系和三元组标注的纯前段工具。具有使用简单的特点，采用网页的形式，使用浏览器便可运行。标注过程、结果直观，易后处理。基本不用配置，快速上手。[试一试](https://freeshman.github.io/LAnn/LittleAnn.html)

## LAnn读取文件
标注工具可以直接读取：
- 原始文本
- BIO命名实体标注后的文本
- LAnn标注过的文本
## 标注流程
### 实体（关系）的标注或取消：
鼠标选中文字，点击界面右边的实体（关系）按钮，完成标注；或点击取消按钮消除先前的标注。
### 三元组的标注：
鼠标分别依次点击SPO，完成三元组的标注。在选择三元组时，“已选中”标签会变成粉红色进行提示。如果点击错误，可点击取消；已标注完成的三元组暂时无法取消标注，请谨慎标注，也可按照标注格式在标注结果中自行删除。
## 标注格式
语料文本的标注结果文件（.lann）每行为一个字符，包含三列，每列用”\t“隔开，分别对应字符域、实体关系域和三元组域。

- 字符域：为统一格式和方便预览，原始文本的换行符“\n”用“_换行符_”代替。
- 实体关系域：采用BIO标注方式。
- 三元组域：包含相同S的三元组都记录在S首字符那一行，三元组之间采用“;”相隔，方便分割；SPO用“>”相隔。不构成三元组的字符该域为“X”。

## TODO

- [ ] 加入分词
- [ ] 智能算法辅助标注
- [ ] 翻译为英文版
