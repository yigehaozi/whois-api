# whois-api
获取域名原始whois并翻译成中文

* 支持的后缀列表：<a href="https://whois.api.ssss.ss/">https://whois.api.ssss.ss/</a>
* api文档: <a href="https://apifox.com/apidoc/shared/f0a610da-db6c-48e6-8c72-fcbde0636d2f/275006680e0">https://apifox.com/apidoc/shared/f0a610da-db6c-48e6-8c72-fcbde0636d2f/275006680e0</a>

---
title: whois翻译项目
language_tabs:
  - shell: Shell
  - http: HTTP
  - javascript: JavaScript
  - ruby: Ruby
  - python: Python
  - php: PHP
  - java: Java
  - go: Go
toc_footers: []
includes: []
search: true
code_clipboard: true
highlight_theme: darkula
headingLevel: 2
generator: "@tarslib/widdershins v4.0.29"

---

# 个人项目

Base URLs:

* 体验环境: <a href="https://petstore-demo.apifox.com">https://petstore-demo.apifox.com</a>

# Authentication

# whois

## POST whois（生产环境） 

POST /public/

> Body 请求参数

```
string

```

### 请求参数

|名称|位置|类型|必选|说明|
|---|---|---|---|---|
|Content-Type|header|string| 否 |none|
|Accept|header|string| 否 |none|
|body|body|string| 否 |none|

> 返回示例

> 200 Response

```json
{
  "domain": {
    "域名": "EXAMPLE.COM",
    "注册域名ID": "2336799_DOMAIN_COM-VRSN",
    "Unicode域名": "例子.com"
  },
  "registrar": {
    "名称": "Example Registrar, LLC",
    "组织": "Example Group International",
    "ID": "1234",
    "IANA_ID": "9999",
    "网站": "http://www.example-registrar.com",
    "传统WHOIS服务器": "whois.example-registrar.com",
    "滥用举报邮箱": "abuse@example-registrar.com",
    "滥用举报电话": "+1.5555551212",
    "街道地址": "123 Registrar Street",
    "城市": "Registrarville",
    "城市中文": "注册商城",
    "邮政编码": "90210",
    "国家": "US",
    "国家中文": "美国"
  },
  "dates": {
    "注册日期": "1995年08月14日 04:00:00",
    "到期日期": "2023年08月13日 04:00:00",
    "更新日期": "2022年07月28日 09:12:34",
    "RDAP数据更新时间": "2022年06月25日 12:00:00"
  },
  "status": {
    "原始状态": "clientTransferProhibited https://icann.org/epp#clientTransferProhibited",
    "主要状态": "注册商禁止转移，https://icann.org/epp#clientTransferProhibited",
    "状态说明": "域名注册商已禁止该域名转移到其他注册商",
    "所有状态码": [
      "clientTransferProhibited",
      "clientUpdateProhibited",
      "clientDeleteProhibited",
      "serverTransferProhibited",
      "registryLock"
    ],
    "中文状态": [
      "注册商禁止转移",
      "注册商禁止更新",
      "注册商禁止删除",
      "注册局禁止转移",
      "注册局锁定"
    ]
  },
  "nameservers": {
    "DNS列表": [
      "NS1.EXAMPLE.COM",
      "NS2.EXAMPLE.COM",
      "NS3.EXAMPLE.COM",
      "NS4.EXAMPLE.COM"
    ],
    "DNSSEC": "已签名"
  },
  "registrant": {
    "姓名": "Example Registrant",
    "组织": "Example Organization",
    "ID": "5372809_CONTACT",
    "电子邮件": "contact@example.com",
    "电话": "+1.5555551234",
    "街道": "123 Example Street",
    "城市": "Anytown",
    "城市中文": "安尼镇",
    "省份": "CA",
    "省份中文": "加利福尼亚州",
    "邮编": "90210",
    "地址": "123 Example Street, Anytown, CA 90210",
    "地址中文": "123 Example Street，安尼镇，加利福尼亚州 90210",
    "国家": "US",
    "国家中文": "美国"
  },
  "admin": {
    "姓名": "Admin Contact",
    "组织": "Example Admin Org",
    "ID": "5372810_CONTACT",
    "电子邮件": "admin@example.com",
    "电话": "+1.5555551235",
    "街道": "456 Admin Street",
    "城市": "Adminville",
    "城市中文": "管理镇",
    "省份": "NY",
    "省份中文": "纽约州",
    "邮编": "10001",
    "地址": "456 Admin Street, Adminville, NY 10001",
    "地址中文": "456 Admin Street，管理镇，纽约州 10001",
    "国家": "US",
    "国家中文": "美国"
  },
  "tech": {
    "姓名": "Tech Contact",
    "组织": "Example Tech Support",
    "ID": "5372811_CONTACT",
    "电子邮件": "tech@example.com",
    "电话": "+1.5555551236",
    "街道": "789 Tech Avenue",
    "城市": "Silicon Valley",
    "城市中文": "硅谷",
    "省份": "CA",
    "省份中文": "加利福尼亚州",
    "邮编": "94043",
    "地址": "789 Tech Avenue, Silicon Valley, CA 94043",
    "地址中文": "789 Tech Avenue，硅谷，加利福尼亚州 94043",
    "国家": "US",
    "国家中文": "美国"
  },
  "billing": {
    "姓名": "Billing Contact",
    "组织": "Example Billing Department",
    "ID": "5372812_CONTACT",
    "电子邮件": "billing@example.com",
    "电话": "+1.5555551237",
    "地址": "321 Billing Blvd, Finance City, TX 75001",
    "地址中文": "321 Billing Blvd，金融城，德克萨斯州 75001",
    "国家": "US",
    "国家中文": "美国"
  },
  "performance": {
    "总耗时": "1234ms",
    "查询时间": "765ms",
    "解析时间": "158ms",
    "翻译时间": "311ms"
  },
  "copyright": "6ke论坛·人皇 © 专业WHOIS解决方案 | 2024-03-22 15:30:45"
}
```

> 400 Response

```json
{
  "error": {
    "code": 400,
    "message": "缺少必要参数: domain"
  }
}
```

> 401 Response

```json
{
  "error": {
    "code": 401,
    "message": "无效的API密钥"
  }
}
```

> 404 Response

```json
{
  "error": {
    "code": 404,
    "message": "未找到域名信息，域名可能不存在或无法解析"
  }
}
```

> 429 Response

```json
{
  "error": {
    "code": 429,
    "message": "查询请求超过限制，请稍后再试",
    "reset_time": "2024-03-22 15:45:30"
  }
}
```

> 500 Response

```json
{
  "error": {
    "code": 500,
    "message": "服务器内部错误，请联系管理员"
  }
}
```

### 返回结果

|状态码|状态码含义|说明|数据模型|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|none|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|none|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|none|Inline|
|429|[Too Many Requests](https://tools.ietf.org/html/rfc6585#section-4)|none|Inline|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|none|Inline|

### 返回数据结构

状态码 **200**

|名称|类型|必选|约束|中文名|说明|
|---|---|---|---|---|---|
|» domain|object|false|none||none|
|»» 域名|string|true|none||none|
|»» 注册域名ID|string|false|none||none|
|»» Unicode域名|string|false|none||none|
|» registrar|object|false|none||none|
|»» 名称|string|false|none||none|
|»» 组织|string|false|none||none|
|»» ID|string|false|none||none|
|»» IANA_ID|string|false|none||none|
|»» 网站|string|false|none||none|
|»» 传统WHOIS服务器|string|false|none||none|
|»» 滥用举报邮箱|string|false|none||none|
|»» 滥用举报电话|string|false|none||none|
|»» 街道地址|string|false|none||none|
|»» 城市|string|false|none||none|
|»» 城市中文|string|false|none||none|
|»» 邮政编码|string|false|none||none|
|»» 国家|string|false|none||none|
|»» 国家中文|string|false|none||none|
|» dates|object|false|none||none|
|»» 注册日期|string|false|none||none|
|»» 到期日期|string|false|none||none|
|»» 更新日期|string|false|none||none|
|»» 人皇数据更新时间|string|false|none||none|
|» status|object|false|none||none|
|»» 原始状态|string|false|none||none|
|»» 主要状态|string|false|none||none|
|»» 状态说明|string|false|none||none|
|»» 所有状态码|[string]|false|none||none|
|»» 中文状态|[string]|false|none||none|
|» nameservers|object|false|none||none|
|»» DNS列表|[string]|false|none||none|
|»» DNSSEC|string|false|none||none|
|» registrant|object|false|none||none|
|»» 姓名|string|false|none||none|
|»» 组织|string|false|none||none|
|»» ID|string|false|none||none|
|»» 电子邮件|string|false|none||none|
|»» 电话|string|false|none||none|
|»» 街道|string|false|none||none|
|»» 城市|string|false|none||none|
|»» 城市中文|string|false|none||none|
|»» 省份|string|false|none||none|
|»» 省份中文|string|false|none||none|
|»» 邮编|string|false|none||none|
|»» 地址|string|false|none||none|
|»» 地址中文|string|false|none||none|
|»» 国家|string|false|none||none|
|»» 国家中文|string|false|none||none|
|» admin|object|false|none||none|
|»» 姓名|string|false|none||none|
|»» 组织|string|false|none||none|
|»» ID|string|false|none||none|
|»» 电子邮件|string|false|none||none|
|»» 电话|string|false|none||none|
|»» 街道|string|false|none||none|
|»» 城市|string|false|none||none|
|»» 城市中文|string|false|none||none|
|»» 省份|string|false|none||none|
|»» 省份中文|string|false|none||none|
|»» 邮编|string|false|none||none|
|»» 地址|string|false|none||none|
|»» 地址中文|string|false|none||none|
|»» 国家|string|false|none||none|
|»» 国家中文|string|false|none||none|
|» tech|object|false|none||none|
|»» 姓名|string|false|none||none|
|»» 组织|string|false|none||none|
|»» ID|string|false|none||none|
|»» 电子邮件|string|false|none||none|
|»» 电话|string|false|none||none|
|»» 街道|string|false|none||none|
|»» 城市|string|false|none||none|
|»» 城市中文|string|false|none||none|
|»» 省份|string|false|none||none|
|»» 省份中文|string|false|none||none|
|»» 邮编|string|false|none||none|
|»» 地址|string|false|none||none|
|»» 地址中文|string|false|none||none|
|»» 国家|string|false|none||none|
|»» 国家中文|string|false|none||none|
|» billing|object|false|none||none|
|»» 姓名|string|false|none||none|
|»» 组织|string|false|none||none|
|»» ID|string|false|none||none|
|»» 电子邮件|string|false|none||none|
|»» 电话|string|false|none||none|
|»» 地址|string|false|none||none|
|»» 地址中文|string|false|none||none|
|»» 国家|string|false|none||none|
|»» 国家中文|string|false|none||none|
|» performance|object|false|none||none|
|»» 总耗时|string|true|none||none|
|»» 查询时间|string|true|none||none|
|»» 解析时间|string|true|none||none|
|»» 翻译时间|string|true|none||none|
|» copyright|string|true|none||none|

状态码 **400**

|名称|类型|必选|约束|中文名|说明|
|---|---|---|---|---|---|
|» error|object|true|none||none|
|»» code|integer|true|none||none|
|»» message|string|true|none||none|

状态码 **401**

|名称|类型|必选|约束|中文名|说明|
|---|---|---|---|---|---|
|» error|object|true|none||none|
|»» code|integer|true|none||none|
|»» message|string|true|none||none|

状态码 **404**

|名称|类型|必选|约束|中文名|说明|
|---|---|---|---|---|---|
|» error|object|true|none||none|
|»» code|integer|true|none||none|
|»» message|string|true|none||none|

状态码 **429**

|名称|类型|必选|约束|中文名|说明|
|---|---|---|---|---|---|
|» error|object|true|none||none|
|»» code|integer|true|none||none|
|»» message|string|true|none||none|
|»» reset_time|string|true|none||none|

状态码 **500**

|名称|类型|必选|约束|中文名|说明|
|---|---|---|---|---|---|
|» error|object|true|none||none|
|»» code|integer|true|none||none|
|»» message|string|true|none||none|

# 数据模型

