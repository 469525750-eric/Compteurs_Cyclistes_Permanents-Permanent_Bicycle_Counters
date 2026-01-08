
This project is designed as a continuous monitoring system rather than a one-off analysis.
SQL is used to enforce data integrity and maintain historical state, while Python handles anomaly detection and decision logic.
Visualization focuses on surfacing actionable, location-aware signals rather than exploratory analysis.

**The goal of this project is not to evaluate policy effectiveness, but to provide continuous operational visibility into active transportation infrastructure.
By transforming raw sensor data into location-aware monitoring signals, the system enables earlier detection of unexpected changes, improved data reliability, and more informed follow-up investigations.**

由于只有一个dataset而且没有很多可以做a/b testing 对比的数据，不能做太多事情。如果有更多的数据比如这几个renovated road (for wider bike lane)看起效程度，会对政策有个更准确的回报评估，也能起到支持政策总结的效果。(source: https://mtlplanifmobilit.maps.arcgis.com/apps/instant/interactivelegend/index.html?appid=0394f5c5974e40a0ae9eac91314c031a&locale=en)
如果你真的要做「城市转型 / 环保成功」你至少需要 5 类数据
① 自行车使用量（你现在只有这一类的一部分）
但还要：BIXI 使用量、私人 vs 共享区分（理想）
② 对照交通方式（极其关键）
汽车流量、公交乘客量、地铁刷卡量
👉 否则你不知道：
“骑车多了，是不是只是因为车更堵？”
③ 政策与基础设施时间线（必须）
哪条路什么时候：
扩建、改造、禁车、明确的 intervention date
④ 强 confounders（不可缺）
天气（温度、降雨、降雪）、油价、人口变化、远程办公比例（疫情后）
⑤ 空间对照（不是 optional）
类似但未改造的路段、同一行政区内的对照

方法层面你才“有资格”谈政策效果
方法（至少一个）：
Difference-in-Differences (DiD)
Interrupted Time Series
Synthetic Control
⚠️ 这已经是社会科学 / 经济学项目，不是 monitoring 项目。太大了。目前不支持。这一段不可行性可以用于面试说明。
<img width="1361" height="807" alt="Screenshot 2026-01-07 at 22 10 51" src="https://github.com/user-attachments/assets/1c6da1cc-01cd-46b9-8bed-996178495cfa" />
