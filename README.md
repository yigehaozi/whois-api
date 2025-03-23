# whois-api
获取域名原始whois并翻译成中文


{
  "openapi": "3.0.1",
  "info": {
    "title": "个人项目",
    "description": "",
    "version": "1.0.0"
  },
  "tags": [
    {
      "name": "whois"
    },
    {
      "name": "域名"
    }
  ],
  "paths": {
    "/public/": {
      "post": {
        "summary": "whois（生产环境） ",
        "deprecated": false,
        "description": "",
        "tags": [
          "whois",
          "域名",
          "whois"
        ],
        "parameters": [
          {
            "name": "Content-Type",
            "in": "header",
            "description": "",
            "required": false,
            "example": "application/json",
            "schema": {
              "type": "string"
            }
          },
          {
            "name": "Accept",
            "in": "header",
            "description": "",
            "required": false,
            "example": "application/json",
            "schema": {
              "type": "string"
            }
          }
        ],
        "requestBody": {
          "content": {
            "text/plain": {
              "schema": {
                "type": "string"
              },
              "examples": {}
            }
          }
        },
        "responses": {
          "200": {
            "description": "",
            "content": {
              "application/json": {
                "schema": {
                  "type": "object",
                  "properties": {
                    "domain": {
                      "type": "object",
                      "properties": {
                        "域名": {
                          "type": "string"
                        },
                        "注册域名ID": {
                          "type": "string"
                        },
                        "Unicode域名": {
                          "type": "string"
                        }
                      },
                      "required": [
                        "域名"
                      ]
                    },
                    "registrar": {
                      "type": "object",
                      "properties": {
                        "名称": {
                          "type": "string"
                        },
                        "组织": {
                          "type": "string"
                        },
                        "ID": {
                          "type": "string"
                        },
                        "IANA_ID": {
                          "type": "string"
                        },
                        "网站": {
                          "type": "string"
                        },
                        "传统WHOIS服务器": {
                          "type": "string"
                        },
                        "滥用举报邮箱": {
                          "type": "string"
                        },
                        "滥用举报电话": {
                          "type": "string"
                        },
                        "街道地址": {
                          "type": "string"
                        },
                        "城市": {
                          "type": "string"
                        },
                        "城市中文": {
                          "type": "string"
                        },
                        "邮政编码": {
                          "type": "string"
                        },
                        "国家": {
                          "type": "string"
                        },
                        "国家中文": {
                          "type": "string"
                        }
                      }
                    },
                    "dates": {
                      "type": "object",
                      "properties": {
                        "注册日期": {
                          "type": "string"
                        },
                        "到期日期": {
                          "type": "string"
                        },
                        "更新日期": {
                          "type": "string"
                        },
                        "人皇数据更新时间": {
                          "type": "string"
                        }
                      }
                    },
                    "status": {
                      "type": "object",
                      "properties": {
                        "原始状态": {
                          "type": "string"
                        },
                        "主要状态": {
                          "type": "string"
                        },
                        "状态说明": {
                          "type": "string"
                        },
                        "所有状态码": {
                          "type": "array",
                          "items": {
                            "type": "string"
                          }
                        },
                        "中文状态": {
                          "type": "array",
                          "items": {
                            "type": "string"
                          }
                        }
                      }
                    },
                    "nameservers": {
                      "type": "object",
                      "properties": {
                        "DNS列表": {
                          "type": "array",
                          "items": {
                            "type": "string"
                          }
                        },
                        "DNSSEC": {
                          "type": "string"
                        }
                      }
                    },
                    "registrant": {
                      "type": "object",
                      "properties": {
                        "姓名": {
                          "type": "string"
                        },
                        "组织": {
                          "type": "string"
                        },
                        "ID": {
                          "type": "string"
                        },
                        "电子邮件": {
                          "type": "string"
                        },
                        "电话": {
                          "type": "string"
                        },
                        "街道": {
                          "type": "string"
                        },
                        "城市": {
                          "type": "string"
                        },
                        "城市中文": {
                          "type": "string"
                        },
                        "省份": {
                          "type": "string"
                        },
                        "省份中文": {
                          "type": "string"
                        },
                        "邮编": {
                          "type": "string"
                        },
                        "地址": {
                          "type": "string"
                        },
                        "地址中文": {
                          "type": "string"
                        },
                        "国家": {
                          "type": "string"
                        },
                        "国家中文": {
                          "type": "string"
                        }
                      }
                    },
                    "admin": {
                      "type": "object",
                      "properties": {
                        "姓名": {
                          "type": "string"
                        },
                        "组织": {
                          "type": "string"
                        },
                        "ID": {
                          "type": "string"
                        },
                        "电子邮件": {
                          "type": "string"
                        },
                        "电话": {
                          "type": "string"
                        },
                        "街道": {
                          "type": "string"
                        },
                        "城市": {
                          "type": "string"
                        },
                        "城市中文": {
                          "type": "string"
                        },
                        "省份": {
                          "type": "string"
                        },
                        "省份中文": {
                          "type": "string"
                        },
                        "邮编": {
                          "type": "string"
                        },
                        "地址": {
                          "type": "string"
                        },
                        "地址中文": {
                          "type": "string"
                        },
                        "国家": {
                          "type": "string"
                        },
                        "国家中文": {
                          "type": "string"
                        }
                      }
                    },
                    "tech": {
                      "type": "object",
                      "properties": {
                        "姓名": {
                          "type": "string"
                        },
                        "组织": {
                          "type": "string"
                        },
                        "ID": {
                          "type": "string"
                        },
                        "电子邮件": {
                          "type": "string"
                        },
                        "电话": {
                          "type": "string"
                        },
                        "街道": {
                          "type": "string"
                        },
                        "城市": {
                          "type": "string"
                        },
                        "城市中文": {
                          "type": "string"
                        },
                        "省份": {
                          "type": "string"
                        },
                        "省份中文": {
                          "type": "string"
                        },
                        "邮编": {
                          "type": "string"
                        },
                        "地址": {
                          "type": "string"
                        },
                        "地址中文": {
                          "type": "string"
                        },
                        "国家": {
                          "type": "string"
                        },
                        "国家中文": {
                          "type": "string"
                        }
                      }
                    },
                    "billing": {
                      "type": "object",
                      "properties": {
                        "姓名": {
                          "type": "string"
                        },
                        "组织": {
                          "type": "string"
                        },
                        "ID": {
                          "type": "string"
                        },
                        "电子邮件": {
                          "type": "string"
                        },
                        "电话": {
                          "type": "string"
                        },
                        "地址": {
                          "type": "string"
                        },
                        "地址中文": {
                          "type": "string"
                        },
                        "国家": {
                          "type": "string"
                        },
                        "国家中文": {
                          "type": "string"
                        }
                      }
                    },
                    "performance": {
                      "type": "object",
                      "properties": {
                        "总耗时": {
                          "type": "string"
                        },
                        "查询时间": {
                          "type": "string"
                        },
                        "解析时间": {
                          "type": "string"
                        },
                        "翻译时间": {
                          "type": "string"
                        }
                      },
                      "required": [
                        "总耗时",
                        "查询时间",
                        "解析时间",
                        "翻译时间"
                      ]
                    },
                    "copyright": {
                      "type": "string"
                    }
                  },
                  "required": [
                    "copyright"
                  ]
                },
                "example": {
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
              }
            },
            "headers": {}
          },
          "400": {
            "description": "",
            "content": {
              "application/json": {
                "schema": {
                  "type": "object",
                  "properties": {
                    "error": {
                      "type": "object",
                      "properties": {
                        "code": {
                          "type": "integer"
                        },
                        "message": {
                          "type": "string"
                        }
                      },
                      "required": [
                        "code",
                        "message"
                      ]
                    }
                  },
                  "required": [
                    "error"
                  ]
                },
                "example": {
                  "error": {
                    "code": 400,
                    "message": "缺少必要参数: domain"
                  }
                }
              }
            },
            "headers": {}
          },
          "401": {
            "description": "",
            "content": {
              "application/json": {
                "schema": {
                  "type": "object",
                  "properties": {
                    "error": {
                      "type": "object",
                      "properties": {
                        "code": {
                          "type": "integer"
                        },
                        "message": {
                          "type": "string"
                        }
                      },
                      "required": [
                        "code",
                        "message"
                      ]
                    }
                  },
                  "required": [
                    "error"
                  ]
                },
                "example": {
                  "error": {
                    "code": 401,
                    "message": "无效的API密钥"
                  }
                }
              }
            },
            "headers": {}
          },
          "404": {
            "description": "",
            "content": {
              "application/json": {
                "schema": {
                  "type": "object",
                  "properties": {
                    "error": {
                      "type": "object",
                      "properties": {
                        "code": {
                          "type": "integer"
                        },
                        "message": {
                          "type": "string"
                        }
                      },
                      "required": [
                        "code",
                        "message"
                      ]
                    }
                  },
                  "required": [
                    "error"
                  ]
                },
                "example": {
                  "error": {
                    "code": 404,
                    "message": "未找到域名信息，域名可能不存在或无法解析"
                  }
                }
              }
            },
            "headers": {}
          },
          "429": {
            "description": "",
            "content": {
              "application/json": {
                "schema": {
                  "type": "object",
                  "properties": {
                    "error": {
                      "type": "object",
                      "properties": {
                        "code": {
                          "type": "integer"
                        },
                        "message": {
                          "type": "string"
                        },
                        "reset_time": {
                          "type": "string"
                        }
                      },
                      "required": [
                        "code",
                        "message",
                        "reset_time"
                      ]
                    }
                  },
                  "required": [
                    "error"
                  ]
                },
                "example": {
                  "error": {
                    "code": 429,
                    "message": "查询请求超过限制，请稍后再试",
                    "reset_time": "2024-03-22 15:45:30"
                  }
                }
              }
            },
            "headers": {}
          },
          "500": {
            "description": "",
            "content": {
              "application/json": {
                "schema": {
                  "type": "object",
                  "properties": {
                    "error": {
                      "type": "object",
                      "properties": {
                        "code": {
                          "type": "integer"
                        },
                        "message": {
                          "type": "string"
                        }
                      },
                      "required": [
                        "code",
                        "message"
                      ]
                    }
                  },
                  "required": [
                    "error",
                    "01JPYWG1K9T6NQ32765Y58KBVV"
                  ]
                },
                "example": {
                  "error": {
                    "code": 500,
                    "message": "服务器内部错误，请联系管理员"
                  }
                }
              }
            },
            "headers": {}
          },
          "x-200-2": {
            "description": "",
            "content": {
              "application/json": {
                "schema": {
                  "type": "object",
                  "properties": {
                    "status": {
                      "type": "string"
                    },
                    "data": {
                      "type": "object",
                      "properties": {
                        "domain": {
                          "type": "object",
                          "properties": {
                            "域名": {
                              "type": "string"
                            },
                            "状态": {
                              "type": "string"
                            },
                            "查询结果": {
                              "type": "string"
                            },
                            "详细信息": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "域名",
                            "状态",
                            "查询结果",
                            "详细信息"
                          ]
                        },
                        "performance": {
                          "type": "object",
                          "properties": {
                            "总耗时": {
                              "type": "string"
                            },
                            "查询时间": {
                              "type": "string"
                            },
                            "解析时间": {
                              "type": "string"
                            },
                            "翻译时间": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "总耗时",
                            "查询时间",
                            "解析时间",
                            "翻译时间"
                          ]
                        },
                        "copyright": {
                          "type": "string"
                        }
                      },
                      "required": [
                        "domain",
                        "performance",
                        "copyright"
                      ]
                    }
                  },
                  "required": [
                    "status",
                    "data"
                  ]
                },
                "example": {
                  "status": "success",
                  "data": {
                    "domain": {
                      "域名": "FGEGESTHTSR.INFO",
                      "状态": "未注册",
                      "查询结果": "该域名目前可注册",
                      "详细信息": "Object not found"
                    },
                    "performance": {
                      "总耗时": "658.33ms",
                      "查询时间": "0ms",
                      "解析时间": "0ms",
                      "翻译时间": "0ms"
                    },
                    "copyright": "6ke论坛·人皇 © 专业WHOIS解决方案 | 2025-03-22 20:43:25"
                  }
                }
              }
            },
            "headers": {}
          }
        },
        "security": []
      }
    }
  },
  "components": {
    "schemas": {},
    "securitySchemes": {}
  },
  "servers": [
    {
      "url": "https://petstore-demo.apifox.com",
      "description": "体验环境"
    }
  ],
  "security": []
}
