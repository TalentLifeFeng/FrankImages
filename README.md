版本 | 作者 | 时间
:-----|:------:|:---:
1.0 | 冯磊 张继文 李响 | 2018/05/09 | 

## 手机管车AI模块卡片组件
### 1，单/多行纯文本。
> componentType:1

- 组件示例：
<html>
<img src="https://raw.githubusercontent.com/TalentLifeFeng/FrankImages/master/1.png" width = "350" height = "105" alt="单/多行纯文本"/>
</html>

- 数据结构：
```
{
	"componentType": 1,
	"data": {
		"title": {
			"text": "您可以这样问我：",
			"fontSize": 15.0,
			"textColor": "#AAAAAA",
			"backgroundColor": "#AAAAAA",
			"borderColor": "#0000FF",
			"borderWidth": 1.0,
			"cornerRadius": 0.0
		},
		"values": [
		    {
				"text": "违章查询",
				"fontSize": 13.0,
				"textColor": "#AAAAAA",
				"backgroundColor": "#AAAAAA",
				"borderColor": "#0000FF",
				"borderWidth": 1.0,
				"cornerRadius": 0.0
			},
			{
				"text": "川A888888到哪里了",
				"fontSize": 13.0,
				"textColor": "#AAAAAA",
				"backgroundColor": "#AAAAAA",
				"borderColor": "#0000FF",
				"borderWidth": 1.0,
				"cornerRadius": 0.0
			}
		]
	}
}
```

- 字段解释：

字段 | 类型 | 必需 | 含义
:-----|:------:|:---:|----:
componentType | int | 是 | 组件的类型（1）
data  | object | 是 | 组件的内容
title | object | 否 | 标题（第一行Label）
values | 数组 | 否 | 标题以下的多个Label
text  | string | 是 | 文本内容
fontSize | int | 否 | 字体大小
textColor | string | 否 | 颜色(hex)
backgroundColor | string | 否 | 颜色(hex)
borderColor | string | 否 | label的border颜色(hex)
borderWidth | float | 否 | label的border宽度
cornerRadius| float | 否 | label的border圆角半径

---

### 2, 车牌号+描述+状态
> componentType:2

- 组件示例：
<html>
<img src="https://raw.githubusercontent.com/TalentLifeFeng/FrankImages/master/2.png" width = "350" height = "45" alt="单/多行纯文本"/>
</html>

- 数据结构：
```
{
  "componentType": 2,
  "data": {
    "title1": {
      "text": "川A123455",
      "fontSize": 15.0,
      "textColor": "#AAAAAA",
      "backgroundColor": "#AAAAAA",
      "borderColor": "#AAAAAA",
      "borderWidth": 1.0,
      "cornerRadius": 3.0
    },
    "title2": {
      "text": "智能管车",
      "fontSize": 12.0,
      "textColor": "#AAAAAA",
      "backgroundColor": "#AAAAAA",
      "borderColor": "#AAAAAA",
      "borderWidth": 1.0,
      "cornerRadius": 3.0
    },
    "title3": {
      "text": "静止",
      "fontSize": 15.0,
      "textColor": "#AAAAAA",
      "backgroundColor": "#AAAAAA",
      "borderColor": "#AAAAAA",
      "borderWidth": 1.0,
      "cornerRadius": 3.0
    }
  }
}
```

- 字段解释：

字段 | 类型 | 必需 | 含义
:-----|:------:|:---:|----:
componentType | int | 是 | 组件的类型（2）
data  | object | 是 | 组件的内容
title1 | object | 否 | 左1 Label
title2 | object | 否 | 左2 Label
title3 | object | 否 | 左3 Label
text  | string | 是 | 文本内容
fontSize | int | 否 | 字体大小
textColor | string | 否 | 颜色(hex)
backgroundColor | string | 否 | 颜色(hex)
borderColor | string | 否 | label的border颜色(hex)
borderWidth | float | 否 | label的border宽度
cornerRadius| float | 否 | label的border圆角半径

---

### 3，icon + 车辆百公里能耗：+ 41.2L + 前往续费
> componentType:3
- 组件示例：

<html>
<img src="https://raw.githubusercontent.com/TalentLifeFeng/FrankImages/master/3.png" width = "350" height = "55" alt="单/多行纯文本"/>
</html>


- 数据结构：
```
{
  "componentType": 3,
  "data": {
    "icon": {
      "url": "http://www.baidu.com/home.png",
      "imageName":"icon1.png",
      "width": 30.0,
      "height": 30.0
    },
    "title1": {
      "text": "百公里能耗：",
      "fontSize": 15.0,
      "textColor": "#AAAAAA",
      "backgroundColor": "#AAAAAA",
      "borderColor": "#AAAAAA",
      "borderWidth": 1.0,
      "cornerRadius": 3.0
    },
    "title2": {
      "text": "14.5L",
      "fontSize": 15.0,
      "textColor": "#FF0000",
      "backgroundColor": "#FFFFFF",
      "borderColor": "#AAAAAA",
      "borderWidth": 1.0,
      "cornerRadius": 3.0
    },
    "title3": {
      "text": "前往续费",
      "fontSize": 15.0,
      "textColor": "#AAAAAA",
      "backgroundColor": "#AAAAAA",
      "borderColor": "#AAAAAA",
      "borderWidth": 1.0,
      "cornerRadius": 3.0
    }
  }
}
```

- 字段解释：

字段 | 类型 | 必需 | 含义
:-----|:------:|:---:|----:
componentType | int | 是 | 组件的类型（3）
data  | object | 是 | 组件的内容
icon | object | 否 | 左1 图片
title1 | object | 否 | 左2 Label
title2 | object | 否 | 左3 Label
title3 | object | 否 | 右1 Label
url | string | 是 | 图片的url
imageName | string | 否 | 本地图片的名字
width | int | 否 | 图片的宽度
height | int | 否 | 图片的高度
text  | string | 是 | 文本内容
fontSize | int | 否 | 字体大小
textColor | string | 否 | 颜色(hex)
backgroundColor | string | 否 | 颜色(hex)
borderColor | string | 否 | label的border颜色(hex)
borderWidth | float | 否 | label的border宽度
cornerRadius| float | 否 | label的border圆角半径

---

### 4,末尾单行文本
> componentType:4

- 组件示例：

<html>
<img src="https://raw.githubusercontent.com/TalentLifeFeng/FrankImages/master/4.png" width = "314" height = "35"/>
</html>

- 数据结构：

```
{
  "componentType": 4,
  "data": {
    "text": "查看其它9辆车",
    "fontSize": 15.0,
    "textColor": "#AAAAAA",
    "backgroundColor": "#AAAAAA",
    "borderColor": "#AAAAAA",
    "borderWidth": 1.0,
    "cornerRadius": 3.0,
    "highLights": [
      {
        "highlightColor": "#FF0000",
        "hightlightRange": [
          4,
          1
        ]
      }
    ]
  }
}
```

- 字段解释：

字段 | 类型 | 必需 | 含义
:-----|:-------:|:---:|:----:
componentType | int | 是 | 组件的类型（4）
data  | object | 是 | 组件的内容
text  | string | 是 | 文本内容
fontSize | int | 否 | 字体大小
textColor | string | 否 | 颜色(hex)
backgroundColor | string | 否 | 颜色(hex)
borderColor | string | 否 | label的border颜色(hex)
borderWidth | float | 否 | label的border宽度
cornerRadius| float | 否 | label的border圆角半径
highLights| Array | 否 | 高亮文本的描述
backgroundColor | string | 否 | 颜色(hex)
hightlightRange | Array | 否 | 第一个元素：起点位置(0开始) 第二个元素：文本长度。图中的“9”,为[4,1]

---

### 5, webView
> componentType:5

- 组件示例：

<html>
<img src="https://raw.githubusercontent.com/TalentLifeFeng/FrankImages/master/5.png" width = "200" height = "200"/>
</html>

- 数据结构：
```
{
  "componentType": 5,
  "data": {
    "url":"http://www.baidu.com",
    "userInteraction":false,
  }
}
```
- 字段解释：

字段 | 类型 | 必需 | 含义
:-----|:-------:|:---:|:----:
componentType | int | 是 | 组件的类型（5）
data  | object | 是 | 组件的内容
url  | string | 是 | webView的链接
userInteraction  | bool | 否 | 是否禁用webView的交互

---

## 一个完整的卡片数据格式：
- 组件示例：

<html>
<img src="https://raw.githubusercontent.com/TalentLifeFeng/FrankImages/master/cardSample.png" width = "212" height = "260"/>

<img src="https://raw.githubusercontent.com/TalentLifeFeng/FrankImages/master/cardAnalyze.png" width = "400" height = "260"/>
</html>

- 数据结构：

```
{
  "card": {
    "itemCount": 4,
    "items": [
      {
        "arrowEnable": false,
        "url": "g7://truckManager/noticeCenter?truckId=34222222",
        "components": [
          {
            "componentType": 5,
            "data": {
              "url": "http://www.baidu.com",
              "userInteraction": false
            }
          }
        ]
      },
      {
        "arrowEnable": false,
        "url": "g7://truckManager/noticeCenter?truckId=34222222",
        "components": [
          {
            "componentType": 2,
            "data": {
              "title1": {
                "text": "川A17951",
                "fontSize": 15.0,
                "textColor": "#AAAAAA"
              },
              "title3": {
                "text": "无法定位",
                "fontSize": 13.0,
                "textColor": "#FF0000",
                "borderColor": "#FF0000",
                "borderWidth": 1.0,
                "cornerRadius": 3.0
              }
            }
          },
          {
            "componentType": 3,
            "data": {
              "icon": {
                "url": "http://www.baidu.com/home.png",
                "imageName": "icon1.png",
                "width": 30.0,
                "height": 30.0
              },
              "title1": {
                "text": "无打卡司机",
                "fontSize": 15.0,
                "textColor": "#AAAAAA"
              }
            }
          },
          {
            "componentType": 3,
            "data": {
              "icon": {
                "url": "http://www.baidu.com/home.png",
                "imageName": "icon1.png",
                "width": 30.0,
                "height": 30.0
              },
              "title1": {
                "text": "暂无地址信息",
                "fontSize": 15.0,
                "textColor": "#AAAAAA"
              }
            }
          },
          {
            "componentType": 3,
            "data": {
              "icon": {
                "url": "http://www.baidu.com/home.png",
                "imageName": "icon1.png",
                "width": 30.0,
                "height": 30.0
              },
              "title1": {
                "text": "最后车辆位置:",
                "fontSize": 15.0,
                "textColor": "#AAAAAA"
              },
              "title2": {
                "text": "--",
                "fontSize": 15.0,
                "textColor": "#AAAAAA"
              }
            }
          }
        ]
      },
      {
        "arrowEnable": false,
        "url": "g7://truckManager/noticeCenter?truckId=34222222",
        "components": [
          {
            "componentType": 4,
            "data": {
              "text": "查看更多",
              "fontSize": 15.0,
              "textColor": "#AAAAAA"
            }
          }
        ]
      }
    ]
  }
}
```

- 字段解释：

字段 | 类型 | 必需 | 含义
:-----|:-------:|:---:|:----:
card | object | 是 | 卡片的信息
itemCount  | int | 是 | 卡片item的个数（行数）
items  | Array | 是 | 卡片所有item（行）的信息
items内部的元素  | object | 是 | 参照前面的组件定义
