# developer-hotspots-summary
> 抓取技术热榜列表，并将文章内容发送给大模型生成摘要，从而达到自动的汇总并解读每日热门技术信息。

## 背景
- 不知道从哪里去获取技术热点信息？
- 工作繁忙没时间了解新知识和技术趋势？
- 近期热点事件老是错过？
- 硬核文章太难或内容太长，没时间深入学习？

## 方案设计 
![方案设计](./picture/image.png)

PS：目前项目暂时没有实现“文章重复数据过滤”、“自定义爬虫”和“内容预处理组件”（可以基于LangChain实现）功能，后续会逐步完善。

## 依赖三方API
- [Tophubdata](https://www.tophubdata.com/): 提供热门榜单数据，现成数据不用自己写爬虫（有一定费用开销）；
- [Moonshot AI](https://platform.moonshot.cn/): 大模型KIMI的API，不支持搜索能力。

## 使用方式
- 修改配置文件config.yaml中的key值, 并按照自己需求调整热榜类型
- 运行main.py程序
```
python3 main.py
```
- 在/result文件下获取生成后文档


License
---

This code is distributed under the MIT license. See `LICENSE` in this directory.