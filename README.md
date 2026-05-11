# Crop-Recommendation-System-Using-Machine-Learning 项目复现

## 1. 项目基本信息
- 对应课程作业登记 Issue: https://github.com/D2RS-2026spring/projects/issues/30
- 项目名称: Crop-Recommendation-System-Using-Machine-Learning 项目的可复现性评估与复现

## 2. 小组成员
- 韩杰 @JieHan369
- 傅垣毓 @FYY0130
- 周蕴熙 @SuperXi-9
- 王子恒 @WZH-303110125

## 3. 原始项目
- 原始项目地址: https://github.com/KRUTHIKTR/Crop-Recommendation-System-Using-Machine-Learning

## 4. 研究目标
本项目围绕原始作物推荐系统开展可复现性评估与复现，检查该项目是否能够在不同环境中完成数据读取、模型训练、结果输出和预测流程，并对结果进行解释。

## 5. 数据来源与预处理
本项目使用原仓库提供的数据集，主要特征包括 N、P、K、temperature、humidity、ph、rainfall，目标变量为 crop label。

预处理工作主要包括：
- 读取原始数据
- 检查数据字段是否完整
- 检查缺失值与异常值情况
- 划分训练集与测试集
- 为后续模型训练准备输入数据

## 6. 数据分析与可视化
本项目对数据进行了基础探索性分析与可视化，包括：
- 各变量的分布情况
- 特征之间的关系
- 不同模型的效果比较
- 结果图表展示

## 7. 模型训练与结果
本项目尝试了多种机器学习模型进行作物推荐预测，包括：
- Logistic Regression
- Gaussian Naive Bayes
- Random Forest
- Support Vector Machine
- AdaBoost

复现结果显示，Gaussian Naive Bayes 模型表现较好，验证集准确率约为 92.53%。

## 8. 结果解读
实验结果表明，原项目在当前数据集和环境下具有较好的可复现性。模型训练流程完整，主要结果能够稳定复现。不同模型在该数据集上的表现存在差异，其中 Gaussian Naive Bayes 和 SVM 表现较优，而部分集成模型效果一般。

## 9. 仓库结构

```text
Crop-Recommendation-System-Using-Machine-Learning/
├── Datasets/
├── Notebook/
├── README.md
├── Requirements.txt
├── Contributing.md
└── crop recommendation model
```

## 10. 复现步骤

1. 下载或克隆本仓库
2. 创建 Python 虚拟环境
3. 安装依赖
4. 打开 Notebook 并按顺序运行
5. 生成结果图表与模型输出
6. 根据 Notebook 中的说明查看分析结论

示例命令：

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
pip install -r Requirements.txt
jupyter notebook
```

## 11. 小组分工

- 韩杰：项目选题、仓库整理、README 编写
- 傅垣毓：数据预处理与结果检查
- 周蕴熙：可视化整理与结果分析
- 王子恒：复现测试与流程记录

## 12. 结论

该项目基本满足结果复现和流程复现要求，但为了更符合课程作业规范，后续仍需继续补充更完整的研究报告说明、成员协作记录以及更加清晰的复现指导。

## 13.测试过程
执行人：王子恒
一、执行情况：
第一步：下载、克隆项目仓库：成功
打开电脑终端：Windows系统右键桌面左下角开始菜单，选择「Windows终端」或「命令提示符（CMD）」；Mac系统直接打开自带的「终端」工具。
选择任意空白磁盘位置作为项目存放路径，无需提前新建文件夹，直接在终端内输入项目官方克隆命令：git clone https://github.com/KRUTHIKTR/Crop-Recommendation-System-Using-Machine-Learning.git，按下回车键执行仓库拉取下载。
等待终端加载完成所有文件，无报错、无中断后，继续输入切换目录命令：cd Crop-Recommendation-System-Using-Machine-Learning，按下回车进入项目根目录。
第二步：安装对应运行环境：成功
保持终端处于项目根目录状态，文档标注可自愿搭建虚拟环境，输入官方创建命令：python -m venv venv，回车创建独立虚拟环境文件夹。
根据系统差异执行激活命令：Windows系统终端输入 venv\Scripts\activate，回车后终端前缀出现「venv」标识，代表环境激活成功。
第三步：安装项目依赖包：成功
直接使用文档提供的官方安装命令，在终端输入：pip install -r requirements.txt，按下回车批量安装项目所需依赖。
第四步：打开运行文件：
保持终端在项目根目录，输入启动命令：jupyter notebook，按下回车启动网页版运行工具。失败，(venv) C:\Users\Lenovo\Crop-Recommendation-System-Using-Machine-Learning>jupyter notebook
'jupyter' 不是内部或外部命令，也不是可运行的程序
等待浏览器自动弹出Jupyter Notebook网页界面，页面自动加载项目所有文件夹及文件。
在网页界面中，找到并点击「Notebook」文件夹，成功定位到项目唯一核心运行文件《Crop recommendation final.ipynb》。
鼠标左键双击该文件，成功打开代码编辑运行界面，文件完整可编辑、可逐单元运行，无文件损坏、无内容缺失、无打开报错问题。
严格依据项目官方README安装与使用说明从零实操，全程不脑补、不私自额外安装程序、不手动修复问题，真实复现情况如下：1. 完成前三步操作后，终端已处于项目根目录且虚拟环境成功激活，严格对照官方文档唯一运行指引，输入启动命令：jupyter notebook 并回车执行。2. 命令执行后终端直接报错：'jupyter' 不是内部或外部命令，也不是可运行的程序或批处理文件，无法启动服务，无服务挂起、无网页链接、无浏览器弹窗。3. 报错核心原因：项目requirements.txt依赖列表未包含jupyter库，官方README文档仅给出启动命令，完全未提前说明需要提前安装jupyter组件，属于严重的文档步骤缺失。4. 对于零基础新手而言，仅依靠项目提供的所有文档和步骤，无法知晓需要额外安装jupyter，无任何合法合规的复现方式，直接卡在项目核心启动环节，无法进入Jupyter工作台、无法打开核心代码文件，后续所有代码运行流程全部中断，本步骤完全无法完成复现。
二、复现过程问题清单：
问题1：运行环境版本说明缺失
项目README仅提供虚拟环境搭建命令，未标注适配的Python版本，零基础新手无法精准匹配运行环境，可能因Python版本不兼容导致后续未知报错。
问题2：核心运行流程说明简略
问题2：核心运行依赖缺失，官方文档步骤断层
项目requirements.txt文件未收录jupyter运行依赖，同时README文档仅直接给出jupyter notebook启动命令，未提前告知用户需要手动安装jupyter组件。零基础新手严格按文档步骤操作会直接触发命令不存在的报错，直接卡死项目运行入口，无任何后续操作空间，是导致项目无法完整复现的核心致命问题。
问题3：实验结果展示不完整
官方仅公示最优模型的准确率数据，未完整展示SVM、AdaBoost、随机森林等其他模型的完整评估结果，新手复现后无法全方位核对所有实验输出，难以判断整体复现效果。
问题4：报错排查说明缺失
项目未提供任何常见运行报错、环境冲突、数据异常的排查方案，新手若出现偶发问题，无解决依据，无法独立完成复现。
三、从第四步继续进行复现：
步骤1：补充安装缺失的核心依赖：成功
保持终端在项目根目录、虚拟环境激活状态，输入以下命令，手动安装 jupyter 组件（弥补项目文档与依赖文件的缺失漏洞）：
pip install jupyter
等待安装完成，无报错、无版本冲突即可进入下一步。
步骤2：启动 Jupyter 服务：成功
依赖安装完成后，继续在当前终端输入官方指定启动命令：
jupyter notebook
按下回车键执行，此时命令可正常识别，终端不会再报错，开始本地服务启动。
步骤3：进入代码运行工作台：失败，成功得到密钥，并可以打开
服务启动成功后，终端会生成带 token 的本地访问链接；http://127.0.0.1:8888，但在输入密钥后显示无法登录，被防火墙隔断了。
直接点击链接，或手动打开浏览器输入 http://127.0.0.1:8888；
若提示密码验证，复制终端的 token 密钥粘贴登录；
成功进入 Jupyter Notebook 网页工作台。

