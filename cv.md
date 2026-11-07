---
layout: page
title: 简历 / CV
permalink: /cv/
---

<div class="cv-section">
<h2>教育背景</h2>
<table class="cv-table">
<tr><td class="cv-period">2025.09 — 至今</td><td><strong>中山大学</strong><br>计算机科学与技术 · 学术型硕士 | 超算中心实验室</td></tr>
<tr><td class="cv-period">2021.09 — 2025.06</td><td><strong>华南理工大学</strong><br>计算机科学与技术 &amp; 金融学 · 双学士<br>GPA: 3.92/4.00 | 双学位班专业第一 | CET-4: 610 | CET-6: 497</td></tr>
</table>
</div>

<div class="cv-section">
<h2>工作经历</h2>

<h3>华为技术有限公司 · ICT BG 数据保护基础软件开发部 <span class="cv-period">2026.07 — 2026.09</span></h3>
<p class="cv-role">AI 算法实习生 | 优秀实习生</p>
<ul>
<li><strong>勒索加密检测：</strong>定位 Shannon 熵 + RNN 无法区分加密与自然高熵数据的根因；引入 NIST SP 800-22 随机性检验，设计 Block → Chunk → Replica 三级检测架构，结合滑动过采样与去冗余筛选 17 维特征，完成 LR 建模。AUC 0.9998，Recall 99.6%，FPR 0.0045%，高熵场景误报率由 35%+ 降至近 0，方案转产并沉淀专利交底书 1 项。</li>
<li><strong>异常检测优化：</strong>基于 CMU 数据重构 9 维分布生成器，以 NSGA-II 多目标优化替代坐标下降。测试集检测率 100%（80/80），Generic 误报率 0%，quiet 场景误报从 100% 降至 0，方案已上线生产。</li>
<li><strong>工程交付：</strong>三仓库构建部署、K8s 换包验证、MyBatis 兼容修复，交付有效代码 3000+ 行。</li>
</ul>

<h3>钛动科技股份有限公司 <span class="cv-period">2026.04 — 2026.06</span></h3>
<p class="cv-role">算法实习生</p>
<ul>
<li>面向 Qwen3.5-27B 多模态微调搭建视频 QA 数据引擎，覆盖 4 类广告视频与 14 个营销理解子任务。</li>
<li>规则层 + Gemini Pro LLM-as-a-Judge 双层质量门控，交付 39,513 条训练样本。</li>
<li>累计处理约 13.4 万次请求、4.80 亿 Token，支持异步并发、重试、断点续跑。</li>
</ul>

<h3>华为技术有限公司 · ICT BG 云计算 · 视频分析服务域 <span class="cv-period">2025.04 — 2025.08</span></h3>
<p class="cv-role">AI 算法实习生（多模态感知与生成方向）</p>
<ul>
<li><strong>D-FINE 异构推理适配：</strong>重构 Deformable Attention，以离散采样替代双线性采样，解决 grid_sample 在 TensorRT 8.x / CANN 6.3 的 Fallback 瓶颈。昇腾吞吐提升约 100%，mAP 损失 &lt;1%。</li>
<li><strong>长尾缺陷合成管线：</strong>Attentive Eraser + Paint-by-Example 方案，车钩托梁折断检测召回率由 85.76% 提升至 99.31%。</li>
<li>整理 8 类模型仓并封装 Docker 镜像。</li>
</ul>
</div>

<div class="cv-section">
<h2>核心项目</h2>

<h3>省算力课题 · GPU/NPU 多租户 LLM 推理资源池化与动态隔离系统 <span class="cv-period">2025.10 — 至今</span></h3>
<p class="cv-role">项目负责人</p>
<ul>
<li>面向 vLLM/SGLang 的底层推理插件，解决多租户共享 GPU/NPU 时 KV Cache、显存带宽和计算资源干扰问题。</li>
<li>跨硬件 Runtime：通过 LD_PRELOAD/dlsym 劫持分别接入 CUDA Runtime 与 ACL Runtime，统一采集资源事件。</li>
<li>最小 5% 粒度的显存/计算资源池化切分，支持严格模式、弹性借用和抢占模式。</li>
<li>完成 GPU/NPU 统一资源池化原型系统、多租户 benchmark、自动化实验和报告生成工具。</li>
</ul>

<h3>古树盘年轮识别系统 <span class="cv-period">2025.06 — 2025.09</span></h3>
<p class="cv-role">项目负责人 | 广州市园科院</p>
<ul>
<li>SAM3-Adapter 分割架构 + CLIP 视觉语义先验特征引导，提升高密度小目标识别精度。</li>
<li>TensorRT FP16 部署，吞吐提升 3 倍、显存下降 60%，实测准确率 &gt;95%。</li>
<li>系统在"全国古树名木保护宣传周"官方活动作为核心成果展出。</li>
</ul>

<h3>安全工程领域事故分析系统 <span class="cv-period">2025.03 — 2025.04</span></h3>
<p class="cv-role">LLM 负责人</p>
<ul>
<li>多模态 RAG 架构：从非结构化事故文本提取风险因子，映射至 FRAM 框架，自动生成贝叶斯网络。</li>
<li>核心算法支撑发表于 Reliability Engineering &amp; System Safety（SCI 一区 Top 期刊）的研究。</li>
</ul>
</div>

<div class="cv-section">
<h2>技术能力</h2>
<ul>
<li><strong>AI Infra：</strong>vLLM / SGLang 推理链路、CUDA / TensorRT、CANN / ACL、Nsight / msprof</li>
<li><strong>AI 工具：</strong>Claude Code、Codex、Cursor、Trae 等辅助开发与调试</li>
<li><strong>算法框架：</strong>PyTorch、ONNX、Docker、K8s</li>
</ul>
</div>

<div class="cv-section">
<h2>竞赛与荣誉</h2>
<ul>
<li><strong>ASC2025 世界大学生超级计算机竞赛</strong> · 二等奖 — AlphaFold3 推理加速、mRNA 位点检测工作流并行优化</li>
<li>国家励志奖学金 · 校级奖学金 · 三好学生</li>
</ul>
</div>
