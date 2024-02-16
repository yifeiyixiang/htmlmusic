#  html音乐播放器 musicPlayer
html音乐播放器 音乐播放器  播放歌曲 支持播放暂停 上一首 下一首切换 支持显示歌曲列表 点击切换歌曲功能

苦于版权原因 可以下载歌曲到本地 通过本项目在线创建自己的歌单实现网页播放和控制

1 歌单上传 歌曲复制到music文件夹 2播放 3 html播放样式  添加列表下拉  音量控制  4 点击选择歌曲播放 

问题1 去除li的marker

如果你使用了marker来修饰列表项，那么`text-decoration: none;`可能会不起作用，因为marker本身就是一个伪元素（pseudo-element），不属于文本内容的一部分。此时，你需要使用CSS伪类（pseudo-class）来选择列表项，并设置其文本装饰。

以下是一个示例的CSS代码，用于设置列表项的文本装饰：

```
 #myList li  {
     list-style-type: none;
}
```

这个CSS代码使用了伪元素选择器（`::marker`）来选择所有列表项的marker。然后，我们将这些marker的文本装饰设置为无（`text-decoration: none;`）。

请注意，这个CSS代码可能不被所有浏览器支持。如果你遇到了兼容性问题，可以考虑使用其他方法来设置列表项的样式，比如通过自定义图片来替代marker。

加列表下啦选项

```
  ulmyList.addClass('active');// 内容栏上移
    ulmyList.removeClass('active');// 内容栏下移
```

添加列表下拉 音量控制 



## 演示效果图：

![](https://img-blog.csdnimg.cn/direct/633092142f39489f8fed619da637c18e.png)
