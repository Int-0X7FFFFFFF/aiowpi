# AIOWPI

## aiohttp based world of warship api
## 以下简称为窝批爱

[![Python 3.8](https://img.shields.io/badge/Python-3.8_|_3.9_|_3.10_|_3.11_|_3.12-blue?style=flat-square&logo=python&logoColor=white)](https://www.python.org/downloads/)
[![GitHub file size in bytes](https://img.shields.io/github/languages/code-size/Int-0X7FFFFFFF/aiowpi?label=Size&logo=hack-the-box&logoColor=white&style=flat-square)](https://github.com/Int-0X7FFFFFFF/aiowpi)
[![PyPI](https://img.shields.io/pypi/v/aiowpi?color=%233775A9&label=PyPI&logo=pypi&logoColor=white&style=flat-square)](https://pypi.org/project/aiowpi/)
[![License](https://img.shields.io/github/license/ArkoClub/async-pixiv?label=License&style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB0PSIxNjUxMjEyODQ2ODY0IiBjbGFzcz0iaWNvbiIgdmlld0JveD0iMCAwIDEwMjQgMTAyNCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHAtaWQ9IjE1MDAiIHdpZHRoPSIzMDAiIGhlaWdodD0iMzAwIj48cGF0aCBkPSJNOTQ3LjIgOTIxLjZsLTg3MC40IDBjLTQyLjM0MjQgMC03Ni44LTM0LjQ1NzYtNzYuOC03Ni44bDAtNjY1LjZjMC00Mi4zNDI0IDM0LjQ1NzYtNzYuOCA3Ni44LTc2LjhsODcwLjQgMGM0Mi4zNDI0IDAgNzYuOCAzNC40NTc2IDc2LjggNzYuOGwwIDY2NS42YzAgNDIuMzQyNC0zNC40NTc2IDc2LjgtNzYuOCA3Ni44ek03Ni44IDE1My42Yy0xNC4xMzEyIDAtMjUuNiAxMS40Njg4LTI1LjYgMjUuNmwwIDY2NS42YzAgMTQuMTMxMiAxMS40Njg4IDI1LjYgMjUuNiAyNS42bDg3MC40IDBjMTQuMTMxMiAwIDI1LjYtMTEuNDY4OCAyNS42LTI1LjZsMC02NjUuNmMwLTE0LjEzMTItMTEuNDY4OC0yNS42LTI1LjYtMjUuNmwtODcwLjQgMHoiIHAtaWQ9IjE1MDEiIGZpbGw9IiNmZmZmZmYiPjwvcGF0aD48cGF0aCBkPSJNNDg2LjQgMzA3LjJsLTMwNy4yIDBjLTE0LjEzMTIgMC0yNS42LTExLjQ2ODgtMjUuNi0yNS42czExLjQ2ODgtMjUuNiAyNS42LTI1LjZsMzA3LjIgMGMxNC4xMzEyIDAgMjUuNiAxMS40Njg4IDI1LjYgMjUuNnMtMTEuNDY4OCAyNS42LTI1LjYgMjUuNnoiIHAtaWQ9IjE1MDIiIGZpbGw9IiNmZmZmZmYiPjwvcGF0aD48cGF0aCBkPSJNNDg2LjQgNDYwLjhsLTMwNy4yIDBjLTE0LjEzMTIgMC0yNS42LTExLjQ2ODgtMjUuNi0yNS42czExLjQ2ODgtMjUuNiAyNS42LTI1LjZsMzA3LjIgMGMxNC4xMzEyIDAgMjUuNiAxMS40Njg4IDI1LjYgMjUuNnMtMTEuNDY4OCAyNS42LTI1LjYgMjUuNnoiIHAtaWQ9IjE1MDMiIGZpbGw9IiNmZmZmZmYiPjwvcGF0aD48cGF0aCBkPSJNNDg2LjQgNTYzLjJsLTMwNy4yIDBjLTE0LjEzMTIgMC0yNS42LTExLjQ2ODgtMjUuNi0yNS42czExLjQ2ODgtMjUuNiAyNS42LTI1LjZsMzA3LjIgMGMxNC4xMzEyIDAgMjUuNiAxMS40Njg4IDI1LjYgMjUuNnMtMTEuNDY4OCAyNS42LTI1LjYgMjUuNnoiIHAtaWQ9IjE1MDQiIGZpbGw9IiNmZmZmZmYiPjwvcGF0aD48cGF0aCBkPSJNNDg2LjQgNjY1LjZsLTMwNy4yIDBjLTE0LjEzMTIgMC0yNS42LTExLjQ2ODgtMjUuNi0yNS42czExLjQ2ODgtMjUuNiAyNS42LTI1LjZsMzA3LjIgMGMxNC4xMzEyIDAgMjUuNiAxMS40Njg4IDI1LjYgMjUuNnMtMTEuNDY4OCAyNS42LTI1LjYgMjUuNnoiIHAtaWQ9IjE1MDUiIGZpbGw9IiNmZmZmZmYiPjwvcGF0aD48cGF0aCBkPSJNNDM1LjIgNzY4bC0yNTYgMGMtMTQuMTMxMiAwLTI1LjYtMTEuNDY4OC0yNS42LTI1LjZzMTEuNDY4OC0yNS42IDI1LjYtMjUuNmwyNTYgMGMxNC4xMzEyIDAgMjUuNiAxMS40Njg4IDI1LjYgMjUuNnMtMTEuNDY4OCAyNS42LTI1LjYgMjUuNnoiIHAtaWQ9IjE1MDYiIGZpbGw9IiNmZmZmZmYiPjwvcGF0aD48cGF0aCBkPSJNOTE4LjY4MTYgMzM1LjA1MjhsLTQxLjYyNTYtMzAuMjU5Mi0xNS45MjMyLTQ4Ljk0NzItNTEuNDU2IDAtNDEuNjI1Ni0zMC4yNTkyLTQxLjYyNTYgMzAuMjU5Mi01MS40NTYgMC0xNS45MjMyIDQ4Ljk0NzItNDEuNjI1NiAzMC4yNTkyIDE1LjkyMzIgNDguOTQ3Mi0xNS45MjMyIDQ4Ljk0NzIgNDEuNjI1NiAzMC4yNTkyIDYuNzU4NCAyMC43ODcyYy0wLjEwMjQgMC44MTkyLTAuMTAyNCAxLjU4NzItMC4xMDI0IDIuNDA2NGwwIDI1NmMwIDEwLjM0MjQgNi4yNDY0IDE5LjcxMiAxNS44MjA4IDIzLjY1NDRzMjAuNTgyNCAxLjc5MiAyNy45MDQtNS41Mjk2bDU4LjY3NTItNTguNjc1MiA1OC42NzUyIDU4LjY3NTJjNC45MTUyIDQuOTE1MiAxMS40MTc2IDcuNTI2NCAxOC4xMjQ4IDcuNDc1MiAzLjI3NjggMCA2LjYwNDgtMC42MTQ0IDkuNzc5Mi0xLjk0NTYgOS41NzQ0LTMuOTQyNCAxNS44MjA4LTEzLjMxMiAxNS44MjA4LTIzLjY1NDRsMC0yNTZjMC0wLjgxOTItMC4wNTEyLTEuNjM4NC0wLjEwMjQtMi40MDY0bDYuNzU4NC0yMC43ODcyIDQxLjYyNTYtMzAuMjU5Mi0xNS45MjMyLTQ4Ljk0NzIgMTUuOTIzMi00OC45NDcyek02NzcuNTI5NiAzNTQuNjExMmwyNC45ODU2LTE4LjE3NiA5LjU3NDQtMjkuMzg4OCAzMC45MjQ4IDAgMjQuOTg1Ni0xOC4xNzYgMjQuOTg1NiAxOC4xNzYgMzAuOTI0OCAwIDkuNTc0NCAyOS4zODg4IDI0Ljk4NTYgMTguMTc2LTkuNTc0NCAyOS4zODg4IDkuNTc0NCAyOS4zODg4LTI0Ljk4NTYgMTguMTc2LTkuNTc0NCAyOS4zODg4LTMwLjkyNDggMC0yNC45ODU2IDE4LjE3Ni0yNC45ODU2LTE4LjE3Ni0zMC45MjQ4IDAtOS41NzQ0LTI5LjM4ODgtMjQuOTg1Ni0xOC4xNzYgOS41NzQ0LTI5LjM4ODgtOS41NzQ0LTI5LjM4ODh6TTc4Ni4xMjQ4IDY0Ny40NzUyYy05Ljk4NC05Ljk4NC0yNi4yMTQ0LTkuOTg0LTM2LjE5ODQgMGwtMzMuMDc1MiAzMy4wNzUyIDAtMTY4LjQ0OCA5LjU3NDQgMCA0MS42MjU2IDMwLjI1OTIgNDEuNjI1Ni0zMC4yNTkyIDkuNTc0NCAwIDAgMTY4LjQ0OC0zMy4wNzUyLTMzLjA3NTJ6IiBwLWlkPSIxNTA3IiBmaWxsPSIjZmZmZmZmIj48L3BhdGg+PC9zdmc+)](./LICENSE)

[![PyPI - Downloads](https://img.shields.io/pypi/dm/aiowpi?color=91A4ED&label=Downloads&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB0PSIxNjUyMjYwMDAwMjU3IiBjbGFzcz0iaWNvbiIgdmlld0JveD0iMCAwIDEwMjQgMTAyNCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHAtaWQ9IjUxNjIiIHdpZHRoPSI1MDAiIGhlaWdodD0iNTAwIj48cGF0aCBkPSJNOTU3LjU0MzkzNyA5NjEuMTMxMTM3IDYyLjg2NTI4MSA5NjEuMTMxMTM3IDYyLjg2NTI4MSA2NTUuNTA5NDg1IDE4OC4yOTgwNjIgNjU1LjUwOTQ4NSAxODguMjk4MDYyIDg1OS4yNDI1ODYgODMyLjE2MDI3NSA4NTkuMjQyNTg2IDgzMi4xNjAyNzUgNjU1LjUwOTQ4NSA5NTcuNTQzOTM3IDY1NS41MDk0ODVaIiBwLWlkPSI1MTYzIiBmaWxsPSIjZmZmZmZmIj48L3BhdGg%2BPHBhdGggZD0iTTc1My4yNzg3MTcgMzYzLjI3ODgxNyA1MTAuMTgwMDUgNzkwLjc0MTQ0NSAyNjcuMDMzMjg3IDM2My4yNzg4MTdaIiBwLWlkPSI1MTY0IiBmaWxsPSIjZmZmZmZmIj48L3BhdGg%2BPHBhdGggZD0iTTQzNC44OTEzMiA2NC4zNTY3NWwxNTAuNTI4MzQyIDAgMCAzMDAuMjU5NTI4LTE1MC41MjgzNDIgMCAwLTMwMC4yNTk1MjhaIiBwLWlkPSI1MTY1IiBmaWxsPSIjZmZmZmZmIj48L3BhdGg%2BPC9zdmc%2B&style=flat-square)](https://pypi.org/project/aiowpi/)
[![View](https://hits.sh/github.com/Int-0X7FFFFFFF/aiowpi.svg?color=7AA3CC&style=flat-square&label=View&logo=data:image/svg+xml;base64,PHN2ZyB0PSIxNjUyMjU5MTQ0MjAzIiBjbGFzcz0iaWNvbiIgdmlld0JveD0iMCAwIDEwMjQgMTAyNCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHAtaWQ9IjM0NjkiIHdpZHRoPSIzMDAiIGhlaWdodD0iMzAwIj48cGF0aCBkPSJNNTEyIDQxNmE5NiA5NiAwIDEgMCAwIDE5MiA5NiA5NiAwIDAgMCAwLTE5MnogbTUxMS45NTIgMTAyLjA2NGMtMC4wMTYtMC40NDgtMC4wNjQtMC44NjQtMC4wOTYtMS4yOTZhOC4xNiA4LjE2IDAgMCAwLTAuMDgtMC42NTZjMC0wLjMyLTAuMDY0LTAuNjI0LTAuMTI4LTAuOTI4LTAuMDMyLTAuMzY4LTAuMDY0LTAuNzM2LTAuMTI4LTEuMDg4LTAuMDMyLTAuMDQ4LTAuMDMyLTAuMDk2LTAuMDMyLTAuMTQ0YTM5LjQ4OCAzOS40ODggMCAwIDAtMTAuNzA0LTIxLjUzNmMtMzIuNjcyLTM5LjYxNi03MS41MzYtNzQuODgtMTExLjA0LTEwNy4wNzItODUuMDg4LTY5LjM5Mi0xODIuNDMyLTEyNy40MjQtMjg5Ljg1Ni0xNTAuOC02Mi4xMTItMTMuNTA0LTEyNC41NzYtMTQuMDY0LTE4Ny4wMDgtMi42NC01Ni43ODQgMTAuMzg0LTExMS41MDQgMzItMTYyLjcyIDU4Ljc4NC04MC4xNzYgNDEuOTItMTUzLjM5MiA5OS42OTYtMjE3LjE4NCAxNjQuNDgtMTEuODA4IDExLjk4NC0yMy41NTIgMjQuMjI0LTM0LjI4OCAzNy4yNDgtMTQuMjg4IDE3LjMyOC0xNC4yODggMzcuODcyIDAgNTUuMjE2IDMyLjY3MiAzOS42MTYgNzEuNTIgNzQuODQ4IDExMS4wNCAxMDcuMDU2IDg1LjEyIDY5LjM5MiAxODIuNDQ4IDEyNy40MDggMjg5Ljg4OCAxNTAuNzg0IDYyLjA5NiAxMy41MDQgMTI0LjYwOCAxNC4wOTYgMTg3LjAwOCAyLjY1NiA1Ni43NjgtMTAuNCAxMTEuNDg4LTMyIDE2Mi43MzYtNTguNzY4IDgwLjE3Ni00MS45MzYgMTUzLjM3Ni05OS42OTYgMjE3LjE4NC0xNjQuNDggMTEuNzkyLTEyIDIzLjUzNi0yNC4yMjQgMzQuMjg4LTM3LjI0OCA1LjcxMi01Ljg3MiA5LjQ1Ni0xMy40NCAxMC43MDQtMjEuNTY4bDAuMDMyLTAuMTI4YTEyLjU5MiAxMi41OTIgMCAwIDAgMC4xMjgtMS4wODhjMC4wNjQtMC4zMDQgMC4wOTYtMC42MjQgMC4xMjgtMC45MjhsMC4wOC0wLjY1NiAwLjA5Ni0xLjI4YzAuMDMyLTAuNjU2IDAuMDQ4LTEuMjk2IDAuMDQ4LTEuOTUybC0wLjA5Ni0xLjk2OHpNNTEyIDcwNGMtMTA2LjAzMiAwLTE5Mi04NS45NTItMTkyLTE5MnM4NS45NTItMTkyIDE5Mi0xOTIgMTkyIDg1Ljk2OCAxOTIgMTkyYzAgMTA2LjA0OC04NS45NjggMTkyLTE5MiAxOTJ6IiBwLWlkPSIzNDcwIiBmaWxsPSIjZmZmZmZmIj48L3BhdGg+PC9zdmc+)](https://hits.sh/github.com/Int-0X7FFFFFFF/aiowpi)



`窝批爱` 是一个基于 aiohttp 的异步战舰世界API库，它兼容多个Python版本，同时拥有较高的效率

## 窝批爱的主要功能

- 异步设计拥有较高的运行效率
- 大概简单易于上手，并且拥有完整的类型标注
- 支持直营服务器 (NA, EU, ASIA, RU(maybe))
- 支持对请求速度进行限制
- 支持动态类型

## 安装

使用 pip 快速安装 `aiowpi`:

```bash
pip install aiowpi
```

## 快速入门
下面是一个简单的例子，允许你使用游戏内使用的名字来搜索玩家的 account_id :
对于请求速率的限制，默认是 10 个请求每秒，这和 WG 文档上面 Standalone applications (独立应用程序) 的最大请求速率一致

```python
import asyncio
from aiowpi import WPIClient, WOWS_ASIA

async def main():
    # Get from wg api full guid
    # Server applications. Request limit per second is set to 20 requests per second.
    # Standalone applications. The limit is set on the number of requests sent from one IP address at the same time and in general equal to 10 requests per second.
    wows_api = WPIClient(
                application_id = "your_application_id",
                max_rate=10,
                rate_time_period=1,
    )
    
    # Search for a player on the Asia server
    player_info = await wows_api.player.search(WOWS_ASIA, "your nick name")
    print(player_info)
asyncio.run(main())
```

## 动态类型
下面是一个简单的例子获取一个玩家的信息:

```python
import asyncio
from aiowpi import WPIClient, WOWS_ASIA

async def main():
    wows_api = WPIClient(application_id = "your_application_id")
    
    # get a player info on the Asia server
    player_info = await wows_api.player.person_data(WOWS_ASIA, 123456)
    print(player_info)
asyncio.run(main())
```

对于支持动态类型的 API 传入一个可迭代对象就可以执行多个玩家的查询


而传入一个 int 如同上面的例子一样则可以查询单个玩家

```python
import asyncio
from aiowpi import WPIClient, WOWS_ASIA

async def main():
    wows_api = WPIClient(application_id = "your_application_id")
    
    # get players info on the Asia server
    player_info = await wows_api.player.person_data(WOWS_ASIA, (123, 456, 789))
    print(player_info)
asyncio.run(main())
```


### [文档参考](https://github.com/ArkoClub/async-pixiv/blob/main/README.md)
