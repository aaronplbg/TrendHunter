---

一、媒体数据表(5张) 

1. ods_social_media (社媒数据) BQ————爬虫、AI填 

| 字段名 | 类型 | 填写说明 | 备注 |
| --- | --- | --- | --- |
| uuid | STRING | 唯一标识 |  |
| task_id | STRING | 关联采集任务ID |  |
| platform | STRING | 固定值 ins |  |
| account_type | STRING | celebrity/fan_account/ blogger |  |
| source_url | STRING | 帖子唯一标识URL |  |
| author_account | STRING | 作者账号名 |  |
| publish_time | TIMESTAMP | 发布时间(Unix秒) |  |
| text_content | STRING | 帖子文字内容 |  |
| image_file_paths | STRING | 图片路径(逗号分隔) |  |
| video_file_path | STRING | 视频路径 |  |
| like_count | INTEGER | 点赞数 |  |
| comment_count | INTEGER | 评论数 |  |
| fetch_time | TIMESTAMP | 爬取时间 |  |
| is_matched | BOOLEAN | 是否已AI分析,默认FALSE | analysis改字段名 |
| matched_at | TIMESTAMP | AI分析完成时间 | analysis改字段名 |
| resaved_image_path | STRING | 转存图片链接 |  |
| resaved_vedio_path | STRING | 转存视频链接 |  |
| image_tag | STRING | 图片标签 |  |
| data_owner | STRING | 数据归属人 |  |
| source_name | STRING | 补充字段,配置权重,填写人名 | 新增字段

 |

2. ods_fashion_media (时尚媒体) BQ———爬虫、AI填 

| 字段名 | 类型 | 填写说明 |
| --- | --- | --- |
| id | STRING | 自动生成UUID |
| source_name | STRING | 配置权重,如:vogue, elle, harper, wwd |
| source_url | STRING | 文章链接,唯一标识 |
| title | STRING | 文章标题 |
| publish_time | TIMESTAMP | 发布时间 |
| text_content | STRING | 文章正文 |
| image_file_path | STRING | 原始图片链接,逗号分隔 |
| resaved_image_path | STRING | 转存图片链接,逗号分隔 |
| video_file_path | STRING | 原始视频链接,逗号分隔 |
| resaved_vedio_path | STRING | 转存视频链接,逗号分隔 |
| fetch_time | TIMESTAMP | 爬取时间 |
| is_matched | BOOLEAN | 是否已AI分析,默认FALSE |
| matched_at | TIMESTAMP | AI分析完成时间

 |

3. ods_ecommerce (电商数据) BQ———爬虫、AI填 

| 字段名 | 类型 | 填写说明 |
| --- | --- | --- |
| id | STRING | 自动生成UUID |
| source_name | STRING | 配置权重,如:farfetch, net-a-porter, ssense, mytheresa |
| source_url | STRING | 商品链接,唯一标识 |
| product_name | STRING | 商品名称 |
| brand | STRING | 品牌名 |
| price | STRING | 价格,如"$1,200" |
| title | STRING | 内容标题 |
| text_content | STRING | 商品描述 |
| image_file_path | STRING | 原始图片链接,逗号分隔 |
| resaved_image_path | STRING | 转存图片链接,逗号分隔 |
| video_file_path | STRING | 原始视频链接,逗号分隔 |
| resaved_vedio_path | STRING | 转存视频链接,逗号分隔 |
| fetch_time | TIMESTAMP | 爬取时间 |
| is_matched | BOOLEAN | 是否已AI分析,默认FALSE |
| matched_at | TIMESTAMP | AI分析完成时间

 |

4. ods_fans (狗仔粉丝网站,待修改) BQ————爬虫、AI填 

| 字段名 | 类型 | 填写说明 |
| --- | --- | --- |
| id | STRING | 自动生成UUID |
| source_name | STRING | 配置权重,填写名人的名字 |
| source_url | STRING | 文章链接,唯一标识 |
| title | STRING | 文章标题 |
| publish_time | TIMESTAMP | 发布时间 |
| text_content | STRING | 文章正文 |
| image_file_path | STRING | 原始图片链接,逗号分隔 |
| resaved_image_path | STRING | 转存图片链接,逗号分隔 |
| video_file_path | STRING | 原始视频链接,逗号分隔 |
| resaved_vedio_path | STRING | 转存视频链接,逗号分隔 |
| fetch_time | TIMESTAMP | 爬取时间 |
| is_matched | BOOLEAN | 是否已AI分析,默认FALSE |
| matched_at | TIMESTAMP | AI分析完成时间

 |

5. ods_brand (品牌官方) BQ———爬虫、AI填 

| 字段名 | 类型 | 填写说明 |
| --- | --- | --- |
| id | STRING | 自动生成UUID |
| source_name | STRING | 来源标识,如:chanel_official, lv_official, gucci_official |
| source_url | STRING | 页面链接,唯一标识 |
| brand | STRING | 品牌名 |
| title | STRING | 内容标题 |
| text_content | STRING | 内容正文 |
| image_file_path | STRING | 原始图片链接,逗号分隔 |
| resaved_image_path | STRING | 转存图片链接,逗号分隔 |
| video_file_path | STRING | 原始视频链接,逗号分隔 |
| resaved_vedio_path | STRING | 转存视频链接,逗号分隔 |
| fetch_time | TIMESTAMP | 爬取时间 |
| is_matched | BOOLEAN | 是否已AI分析,默认FALSE |
| matched_at | TIMESTAMP | AI分析完成时间

 |

---

二、配置表(4张) 

5. raw_standard_products (标准商品库) BQ———爬虫 

| 字段名 | 类型 | 必填 | 填写说明 |
| --- | --- | --- | --- |
| id | STRING |  | 自动生成UUID |
| source_name | STRING |  | 数据来源名称:Bottega Veneta、miumiu等 |
| source_url | STRING |  | 商品原始链接,唯一标识 |
| brand | STRING |  | 品牌名称:Bottega Veneta、miumiu等。注意:数据来源不一定和品牌同名。 |
| product_name | STRING |  | 商品名称(产品名称) |
| price | STRING |  | 价格 |
| product_detail | STRING |  | 产品细节描述 |
| spec | STRING |  | 产品长宽高的描述 |
| material_raw | STRING |  | 网站原始材料名称 |
| image_file_path | STRING |  | 商品图片URL,多个用英文逗号分隔。注意:同一个详情页可能有多种颜色,都要存 |
| image_stored_path | STRING |  | 转存后的图片URL |
| video_file_path | STRING |  | 商品视频URL |
| video_stored_path | STRING |  | 转存后的视频URL |
| fetch_time | TIMESTAMP |  | 采集时间

 |

6. standard_products AI填,AI处理过后的数据存supabase 

| 字段名 | 类型 | 说明 |
| --- | --- | --- |
| id | UUID | 主键,对应 raw_standard_products.id |
| category_id | BIGINT | AI识别的品类ID,关联 category dimensions.id |
| dimensions | JSONB | AI提取的维度值,JSON格式字符串,如: `{"bag_type":"tote","material":"leather","color":"black"}` |
| processed_time | TIMESTAMPTZ | AI 处理时间

 |

7. category_dimensions (品类维度配置) supabase—————根据业务要求填 

| 字段名 | 类型 | 填写说明 |
| --- | --- | --- |
| id | INT64 | 品类ID,如1=包袋,2=鞋履 |
| name | STRING | 品类名称 |
| dimensions | STRING | 维度定义JSON,如 `{"bag_type":["tote","crossbody"],"material":["leather","canvas"]}`

 |

8. fashion_config (时尚表配置,含权重) supabase————根据业务要求填 

| 字段名 | 类型 | 填写说明 |
| --- | --- | --- |
| id | INT64 | 自增ID |
| source_name | STRING | 与4张媒体表的source_name对应,如:vogue, farfetch,某社媒人名 |
| fashion_weight | FLOAT64 | 时尚权重,0-1之间,如0.9 |
| description | STRING | 备注说明

 |

---

三、AI处理表 

9. ai_match 

| 字段名 | 类型 | 说明 | 必要性 |
| --- | --- | --- | --- |
| id | STRING | 自动生成UUID |  |
| source_table | STRING | 来源表名:ods_social_media/ods_fans/ods_fashion_media/ods_ecommerce/ods_brand | 因为5张表是独立的表,各自的id只在表内唯一,不同表之间id可能重复。 |
| source_id | STRING | 来源表的id(外键) | 关联来源表的唯一键,统计时需要 JOIN 获取 source_name/fetch_time |
| standard_product_id | STRING | 匹配到的 standard products.id (外键) | 核心匹配结果,关联标准商品库 |
| confidence | FLOAT64 | 匹配置信度,0-1 | 阿里云图搜返回的置信度,用于筛选可匹配 |
| matched_at | TIMESTAMP | 匹配完成时间 | 记录 AI 处理时间,用于监控和排查

 |

---
