# Primary Care Physician Skills

按儿童、成年人和老年人组织的个人与家庭健康资料检索技能。每个科室为一个独立 skill，使用标准 `SKILL.md`、`agents/openai.yaml` 与 `references/guidelines.md` 结构。

- 内容与文献核验日期：**2026-11-02**。
- 规模：**21 个科室技能、21 份文献清单、4 份导航文档**；另含每个技能的 UI 配置，共 **67 个文件**。
- 文献：**132 条逐项资料**，包括正式指南、专家共识、临床路径、专业专题和患者教育；同一资料可能跨科复用。
- 语言：目录和技能标识使用英文，工作流程与文献说明以中文为主。
- 用途：按问题查找权威资料、核对适用条件、理解检查及医生方案、准备就诊问题。

## Navigation

- [Naming conventions / 命名规范](#naming-conventions--命名规范)
- [Children / 儿童](#children)
- [Adults / 成年人](#adults)
- [Older Adults / 老年人](#older-adults)
- [Skill structure / 技能结构](#skill-structure--技能结构)
- [分类口径](#分类口径)
- [资料类型与阅读顺序](#资料类型与阅读顺序)
- [通用官方入口](#通用官方入口)
- [核验与更新约定](#核验与更新约定)
- [技能使用与维护](#技能使用与维护)

## Naming conventions / 命名规范

三个一级目录按人群命名为 `children/`、`adults/`、`older-adults/`。科室目录使用小写英文与连字符；各科室的 `SKILL.md` frontmatter `name` 与其目录名完全一致，并在全仓库内保持唯一。

科室分类参考国家卫生健康委公开的[《医疗机构诊疗科目名录》](https://www.nhc.gov.cn/fzs/c100048/201808/afa9a6d10b9c4ed3ac36358fc20243ff.shtml)，英文采用通行专科名称。例如 `Otolaryngology` 对应耳鼻咽喉科，`Urology` 对应泌尿外科，`Endocrinology` 对应内分泌科。该名录本次从官方索引核对，正文直连返回 412。

采用 `General Internal Medicine` 对应普通内科；儿童生长发育、营养与常规保健归 `Child Health Care`。这两个英文科室名称分别可在 [Johns Hopkins 内科分科](https://www.hopkinsmedicine.org/medicine)及[上海市儿童医院官方年报](https://www.shchildren.com.cn/Up_Load_Files/files/2025/9/4132548499.pdf)查到。英文技能标识用于本仓库组织，不充当医疗机构登记代码。

儿科使用 `general-pediatrics`、`pediatric-*`、`child-health-care` 等专业名称；成人和老人分别使用 `adult-*` 与 `older-adult-*` 限定人群。哮喘、近视、防龋、三高等专题保留在文献和检索流程中。

## Children

[进入 儿童及青少年技能目录](children/README.md)

| 标准科室与技能入口 | 文献清单 | 重点问题 |
| --- | --- | --- |
| [General Pediatrics（普通儿科）](children/general-pediatrics/SKILL.md) | [guidelines.md](children/general-pediatrics/references/guidelines.md) | 儿童常见发热、一般感染、腹泻、呕吐及综合评估 |
| [Pediatric Pulmonology（儿童呼吸科）](children/pediatric-pulmonology/SKILL.md) | [guidelines.md](children/pediatric-pulmonology/references/guidelines.md) | 咳嗽、喘息、哮喘、肺炎，按儿童年龄分组检索 |
| [Pediatric Ophthalmology（儿童眼科）](children/pediatric-ophthalmology/SKILL.md) | [guidelines.md](children/pediatric-ophthalmology/references/guidelines.md) | 视力筛查、屈光检查、近视发生与进展、专业随访 |
| [Pediatric Dentistry（儿童口腔科）](children/pediatric-dentistry/SKILL.md) | [guidelines.md](children/pediatric-dentistry/references/guidelines.md) | 龋齿风险、含氟防龋、窝沟封闭、刷牙与口腔检查 |
| [Pediatric Otolaryngology（儿童耳鼻咽喉科）](children/pediatric-otolaryngology/SKILL.md) | [guidelines.md](children/pediatric-otolaryngology/references/guidelines.md) | 扁桃体、腺样体、中耳炎、听力、打鼾及睡眠呼吸 |
| [Child Health Care（儿童保健科）](children/child-health-care/SKILL.md) | [guidelines.md](children/child-health-care/references/guidelines.md) | 身高体重、生长曲线、发育监测、青春期与儿童内分泌 |
| [Pediatric Allergy and Immunology（儿童过敏与免疫科）](children/pediatric-allergy-and-immunology/SKILL.md) | [guidelines.md](children/pediatric-allergy-and-immunology/references/guidelines.md) | 鼻炎、食物与药物过敏、过敏评估及相关皮肤问题 |
| [Pediatric Dermatology（儿童皮肤科）](children/pediatric-dermatology/SKILL.md) | [guidelines.md](children/pediatric-dermatology/references/guidelines.md) | 湿疹、皮炎、荨麻疹、感染相关皮疹等 |

## Adults

[进入 成年人技能目录](adults/README.md)

| 标准科室与技能入口 | 文献清单 | 重点问题 |
| --- | --- | --- |
| [General Internal Medicine（普通内科）](adults/adult-general-internal-medicine/SKILL.md) | [guidelines.md](adults/adult-general-internal-medicine/references/guidelines.md) | 一般感冒、急性咳嗽、咽痛、常见感染与综合评估 |
| [Otolaryngology（耳鼻咽喉科）](adults/adult-otolaryngology/SKILL.md) | [guidelines.md](adults/adult-otolaryngology/references/guidelines.md) | 鼻塞、鼻痒、喷嚏、过敏性鼻炎与鼻眼症状 |
| [Ophthalmology（眼科）](adults/adult-ophthalmology/SKILL.md) | [guidelines.md](adults/adult-ophthalmology/references/guidelines.md) | 红眼、结膜炎、过敏相关眼部症状及鉴别资料 |
| [Gynecology（妇科）](adults/adult-gynecology/SKILL.md) | [guidelines.md](adults/adult-gynecology/references/guidelines.md) | 外阴阴道不适、经量异常、更年期及孕期适用边界 |
| [Urology（泌尿外科）](adults/adult-urology/SKILL.md) | [guidelines.md](adults/adult-urology/references/guidelines.md) | 排尿问题、包皮龟头不适与男性勃起功能问题 |
| [Dermatology（皮肤科）](adults/adult-dermatology/SKILL.md) | [guidelines.md](adults/adult-dermatology/references/guidelines.md) | 脚气、常见皮疹、湿疹、接触性皮炎与真菌感染 |
| [Dentistry（口腔科）](adults/adult-dentistry/SKILL.md) | [guidelines.md](adults/adult-dentistry/references/guidelines.md) | 防龋、牙周健康、牙齿清洁、龋损与牙痛资料 |

## Older Adults

[进入 老年人技能目录](older-adults/README.md)

| 标准科室与技能入口 | 文献清单 | 重点问题 |
| --- | --- | --- |
| [Cardiology（心血管内科）](older-adults/older-adult-cardiology/SKILL.md) | [guidelines.md](older-adults/older-adult-cardiology/references/guidelines.md) | 高血压、血脂异常和心血管风险；高血糖关联糖尿病文档 |
| [Pulmonology（呼吸内科）](older-adults/older-adult-pulmonology/SKILL.md) | [guidelines.md](older-adults/older-adult-pulmonology/references/guidelines.md) | 慢阻肺及急性加重、慢性呼吸症状、肺康复与家庭氧疗评估资料 |
| [Endocrinology（内分泌科）](older-adults/older-adult-endocrinology/SKILL.md) | [guidelines.md](older-adults/older-adult-endocrinology/references/guidelines.md) | 糖尿病、低血糖、老年个体化管理及并发症 |
| [Ophthalmology（眼科）](older-adults/older-adult-ophthalmology/SKILL.md) | [guidelines.md](older-adults/older-adult-ophthalmology/references/guidelines.md) | 白内障、青光眼、糖尿病视网膜病变与糖尿病黄斑水肿 |
| [Geriatric Medicine（老年医学科）](older-adults/older-adult-geriatric-medicine/SKILL.md) | [guidelines.md](older-adults/older-adult-geriatric-medicine/references/guidelines.md) | 多病共存、衰弱、跌倒、营养、功能状态和多重用药 |
| [Rheumatology（风湿免疫科）](older-adults/older-adult-rheumatology/SKILL.md) | [guidelines.md](older-adults/older-adult-rheumatology/references/guidelines.md) | 痛风、类风湿关节炎、骨关节炎及其他关节问题 |

## Skill structure / 技能结构

以 `children/pediatric-pulmonology/` 为例：

| 文件 | 标准用途 |
| --- | --- |
| [SKILL.md](children/pediatric-pulmonology/SKILL.md) | YAML frontmatter 仅含 `name`、`description`；正文规定科室查阅流程、资料选择、输出要求与适用边界 |
| [references/guidelines.md](children/pediatric-pulmonology/references/guidelines.md) | 官方资料网址、版本、人群、用途、核验范围、中英文检索词与跨科导航 |
| [agents/openai.yaml](children/pediatric-pulmonology/agents/openai.yaml) | `display_name`、`short_description`、`default_prompt`；默认提示词引用对应 `$skill-name` |

所有科室均通过官方 `skill-creator` 的 `init_skill.py` 初始化，并使用其 `generate_openai_yaml.py` 生成 UI 配置、`quick_validate.py` 检查格式。每个技能只包含实际使用的文件；详细文献按需加载。

## 分类口径

1. **结膜炎放在眼科。** 鼻炎和眼部过敏症状可一起检索，两个文档互相链接，保留各自的检查与鉴别范围。
2. **儿童生长发育单独建档。** 常规生长与发育资料归儿童保健／儿童内分泌；腺样体、扁桃体、听力与睡眠呼吸资料归耳鼻喉科，并建立关联。
3. **“三高”是检索导航标签。** 高血压和血脂异常放在心血管文档，高血糖的详细资料放在糖尿病文档。
4. **人群文件夹用于家庭导航。** 个别指南可能使用 5 岁以下、6–11 岁、12 岁以上、65 岁以上等特定范围；实际使用以原文纳入人群为准。
5. **允许多科室联合检索。** 主要症状对应一个入口，相关专科作为补充；同一病例的病史与已知检查应保持一致。

## 资料类型与阅读顺序

| 类型 | 主要用途 | 阅读时关注什么 |
| --- | --- | --- |
| 正式临床指南／诊疗规范 | 核对评估、检查、治疗及随访的依据 | 适用人群、临床问题、推荐强度、证据质量、版本与状态 |
| 专家共识／立场声明／策略报告 | 了解特定问题的专业建议与实践框架 | 文件具体类型、制定方法、适用条件及证据局限 |
| 医院临床路径 | 了解某个临床场景下的处理流程 | 医疗场景、可用资源和当地实践 |
| 医学知识库 | 了解症状、疾病、检查和治疗的背景 | 审核日期、作者／审稿机制，以及与原始指南的对应关系 |
| 官方患者教育 | 理解疾病、家庭照护、检查准备和就医沟通 | 面向谁、何时寻求帮助、适用地区与更新时间 |

日常阅读可从患者教育或中文知识库开始；需要核对诊疗依据时，回到对应人群的现行正式文件。中国规范与国际资料有差异时，分别记录适用人群、医疗体系、证据时间和药品可用性。

## 通用官方入口

| 来源 | 网址 | 定位 |
| --- | --- | --- |
| 国家卫生健康委医政司 | [政策文件](https://www.nhc.gov.cn/yzygj/c100068/new_list.shtml) · [工作动态](https://www.nhc.gov.cn/yzygj/c100067/new_list.shtml) | 中国官方发布的诊疗指南、方案与规范 |
| 中华医学期刊全文数据库 | [yiigle.com](https://www.yiigle.com/) | 中华医学会系列期刊原始文献与指南共识；全文权限逐篇确认 |
| NICE | [已发布资料](https://www.nice.org.uk/guidance/published) | 英国跨专科指南与相关建议，注意文件类别和更新日期 |
| MSD 默沙东诊疗手册 | [中文专业版与大众版入口](https://www.msdmanuals.cn/) | 中文医学知识库；从首页选择专业版或大众版 |
| NHS | [疾病 A–Z](https://www.nhs.uk/conditions/) | 英国官方患者教育 |
| MedlinePlus | [健康主题](https://medlineplus.gov/healthtopics.html) | 美国国家医学图书馆患者资料与检查／药品导航 |
| 国家药监局 | [药品查询](https://www.nmpa.gov.cn/zwfwqjd/index.html) | 核对药品批准、生产企业、剂型和规格等注册信息 |
| DailyMed | [药品标签检索](https://dailymed.nlm.nih.gov/dailymed/) | 美国在用药品标签；同时核对产品监管状态与中国具体产品说明书 |

## 核验与更新约定

- **已读取网页**：本次可以读取该网页的主体内容；不代表已经阅读目录中的全部下游文件。
- **官方索引／摘要确认**：已从原发布机构、期刊或官方书目确认标题和链接；具体推荐仍需核对全文。
- **需登录／订阅**：仅在网站明确说明或出现实际访问要求时标记，具体权限以单篇文件为准。
- **访问受限**：本次自动访问受到限制；这与链接失效、资料撤回或需要付费是不同情况。
- **中文检索入口**：当专病原文直链未稳定核实时，保留官方目录和准确关键词，不把入口冒充某份指南全文。
- 指南名称中的年份、正式发表时间、网页最后审查时间和检索时间分别记录。搜索引擎的抓取日期不能充当指南年份。
- 保留稳定的官方总目录，同时列出已核实的具体专题链接。每次引用具体建议前重新检查其更新、撤回、被替代或归档状态。
- 公开征求意见稿、在研指南、归档文件应明确标注；其状态不能仅靠文件年代判断。
- 本仓库保存链接与中文导航说明。自动下载、全文入库、再分发及 AI 使用应按各网站许可执行；例如 [AAO 的资料目录](https://www.aao.org/education/guidelines-browse) 明示其内容的 AI 使用限制，应先作为人工查阅入口。

## 技能使用与维护

1. 根据人群、主要问题和任务目的选择一个主科室，按需参考关联科室。
2. 使用该科室 `SKILL.md` 中的流程；只补齐会影响资料选择的关键事实，保留未知项。
3. 区分疾病解释、检查解读、医生方案理解、家庭观察和就诊准备，再选择对应资料类型。
4. 每次引用具体建议时回到原发布方，核对现行版本、适用人群、具体章节和访问状态。
5. 明确区分原文推荐、一般医学解释和基于有限信息的推测；无法读取全文时说明证据缺口。
6. 更新文献时维护对应 `references/guidelines.md`；改变触发范围或工作流时同步维护 `SKILL.md` 与 `agents/openai.yaml`。
7. 保留技能目录名称与 frontmatter `name` 一致，修改路径后同步检查所有目录和文献链接。

原有官方网址与版本说明保留在各科文献中。此仓库只存技能和参考资料，不存个人或家庭的病历信息。
