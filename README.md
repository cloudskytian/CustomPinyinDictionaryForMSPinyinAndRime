# 用于 Rime 和 微软拼音自定义短语 的 CustomPinyinDictionary

fork 自 <https://github.com/wuhgit/CustomPinyinDictionary>

使用 libime 将 CustomPinyinDictionary 转换为 libimetxt 后使用 [深蓝词库转换](https://github.com/studyzy/imewlconverter) 将其转换为 Rime 和 微软拼音自定义短语 格式

利用 Github Action 进行转换与发布

![](https://raw.githubusercontent.com/wuhgit/CustomPinyinDictionary/main/documents/title.png)

<br/>

<div><img src="https://img.shields.io/badge/dynamic/json?style=social&label=%E6%9B%B4%E6%96%B0%E6%97%A5%E6%9C%9F&query=updateDate&url=https%3A%2F%2Fgithub.com%2Fwuhgit%2FCustomPinyinDictionary%2Fraw%2Fmain%2Fstatus.json" align="right">&emsp;&emsp;&emsp;&emsp;<img src="https://img.shields.io/badge/dynamic/json?style=social&label=%E6%95%B0%E6%8D%AE%E6%9B%B4%E6%96%B0%E8%AE%A1%E6%95%B0&query=versionNumber&url=https%3A%2F%2Fgithub.com%2Fwuhgit%2FCustomPinyinDictionary%2Fraw%2Fmain%2Fstatus.json" align="right">&emsp;&emsp;&emsp;&emsp;<img src="https://img.shields.io/badge/dynamic/json?style=social&label=%E8%AF%8D%E6%9D%A1%E6%80%BB%E8%AE%A1&query=totalWords&url=https%3A%2F%2Fgithub.com%2Fwuhgit%2FCustomPinyinDictionary%2Fraw%2Fmain%2Fstatus.json" align="right"></div>

<br/>

---

针对日常输入习惯，当前词库包含了以下内容：

* 人文类
	* 成语
	* 俗语
	* 诗歌
	* 汉语相关词典（感谢[FREEMDICT](https://forum.freemdict.com)）
	* ……
* 地理类
	* 中华人民共和国行政区划，收录`省份、城市、区县、乡镇`四级数据（感谢[Administrative-divisions-of-China](https://github.com/modood/Administrative-divisions-of-China)）
	* 世界主要国家或地区，收录`国名全称、简称、首都`（感谢[wgii](https://github.com/occultskyrong/wgii)）
	* 世界各国和地区名称及一级行政区划（数据来源：[中华人民共和国海关总署](http://online.customs.gov.cn/)）
	* ……
* 生活类
	* 统计用产品分类目录（数据来源：[国家统计局](http://www.stats.gov.cn/)）
	* 商品目录（数据来源：京东、淘宝 等购物网站）
	* 常见人名
	* ……
* 其它
    * 第三方输入法词库
	* ……


> 已对以上所有数据进行去重、精简处理。


---

# 已知问题

由于微软拼音自学习词库上限为两万条，因此仅支持自定义短语，不支持自学习词库，导入自定义短语后会导致该项设置之后卡死无法打开，需要手动清除配置文件才能打开，但输入测试表明导入是生效的

如果要卸载或者更新，把 %APPDATA%\Microsoft\InputMethod\ChsChsPinyinEUDPv1.lex 删掉即可卸载该词库，可以打开自定义词条界面，建议顺便点下清理，然后就可以再导入了

具体可见 <https://github.com/wuhgit/CustomPinyinDictionary/issues/50> 和 <https://www.52pojie.cn/thread-1227015-1-1.html>

# 下载

libimetxt 格式：[CustomPinyinDictionary_libimetxt.txt](https://github.com/cloudskytian/CustomPinyinDictionaryForMSPinyin/releases/latest/download/CustomPinyinDictionary_libimetxt.txt)

Rime：[CustomPinyinDictionary_rime.yaml](https://github.com/cloudskytian/CustomPinyinDictionaryForMSPinyin/releases/latest/download/CustomPinyinDictionary_rime.yaml)

微软拼音自定义短语：[win10mspy.dat](https://github.com/cloudskytian/CustomPinyinDictionaryForMSPinyin/releases/latest/download/win10mspy.dat)

<div><img src="https://fcitx-im.org/fcitx.png" alt="Fcitx5 logo" width="100" align="right"></div>
