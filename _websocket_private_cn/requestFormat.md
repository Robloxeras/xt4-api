---
title: 请求报文格式
position_number: 2
type:
description: |+

parameters:
    -
        name:
        type: string
        mandatory: false
        default:
        description:
        ranges:
content_markdown: |-
    **param结构**

    \{topic\}@\{arg\},\{arg\},…
left_code_blocks:
    -
        code_block: "{\r\n    \"method\": \"subscribe\", \r\n    \"params\": [\r\n        \"{topic}@{arg},{arg}\",    //event\r\n        \"{topic}@{arg}\"\r\n    ], \r\n    \"listenKey\": \"512312356123123123\",   //监听Key，先通过rest接⼝申请\r\n    \"id\": \"{id}\"\r\n}"
        title: 订阅
        language: json
    -
        code_block: |-
            {
                "method": "unsubscribe", 
                "params": [
                    "{topic}@{arg},{arg}",    //event
                    "{topic}@{arg}"
                ], 
                "listenKey": "512312356123123123",   //监听Key，先通过rest接⼝申请
                "id": "{id}"
            }
        title: 取消订阅
        language: json
right_code_blocks:
    -
        code_block:
        title: Response
        language: json
---
