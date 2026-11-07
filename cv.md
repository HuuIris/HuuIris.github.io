---
layout: page
title: CV — Biao Hu
permalink: /cv/
---

<div class="cv-section">
<h2>Education</h2>
<table class="cv-table">
<tr><td class="cv-period">2025.09 — Present</td><td><strong>Sun Yat-sen University</strong><br>M.S. in Computer Science and Technology<br>National Supercomputing Center · Advisor: TBD<br><em>Research: AI Infrastructure & LLM Inference Optimization</em></td></tr>
<tr><td class="cv-period">2021.09 — 2025.06</td><td><strong>South China University of Technology</strong><br>B.Eng. Computer Science & Technology + B.Fin. Finance (Dual Degree)<br>GPA: 3.92/4.00 · <strong>First in dual-degree cohort</strong></td></tr>
</table>
</div>

<div class="cv-section">
<h2>Publications</h2>
<ul>
<li><strong>Biao Hu</strong>, et al. "LLM-based Risk Factor Extraction and Bayesian Network Generation for Safety Engineering." <em>Reliability Engineering & System Safety</em> (SCI Q1, Top Journal). Supporting research — core algorithm development.</li>
<li><strong>Biao Hu</strong>. "GPU/NPU Multi-Tenant LLM Inference Resource Pooling with Dynamic Isolation." Provincial Computing Grant Project. <em>In progress.</em></li>
</ul>
</div>

<div class="cv-section">
<h2>Research Experience</h2>

<h3>Multi-Tenant LLM Inference Resource Pooling <span class="cv-period">2025.10 — Present</span></h3>
<p class="cv-role">Lead Researcher · Provincial Computing Grant</p>
<ul>
<li>Building runtime-level resource virtualization for vLLM/SGLang across CUDA and ACL via LD_PRELOAD/dlsym — no mainline modification</li>
<li>Profiling prefill (compute-bound) vs. decode (memory-bound) stages; identified 127% TPOT p99 degradation under long-context interference</li>
<li>Resource pooling at 5% minimum granularity; near-linear goodput/TTFT scaling with allocated share</li>
<li>Three scheduling modes: strict isolation, elastic borrowing, priority-based preemption</li>
<li>Unified benchmark suite across 2/3/4/8 tenants on Qwen2/2.5/3 model families</li>
</ul>

<h3>Operator-Level Inference Adaptation for Heterogeneous Hardware <span class="cv-period">2025.04 — 2025.08</span></h3>
<p class="cv-role">Research Collaborator</p>
<ul>
<li>Led D-FINE (SOTA detector) adaptation: identified <code>grid_sample</code> fallback on TensorRT 8.x / CANN 6.3 as primary bottleneck</li>
<li>Reformulated deformable attention from bilinear to discrete sampling — ~100% throughput improvement on Ascend CANN 6.3, &lt;1% mAP loss</li>
<li>Backward-compatible with CUDA/TensorRT 8.x for legacy deployment (CUDA 10.1/10.2)</li>
<li>Built long-tail defect synthesis pipeline (Attentive Eraser + Paint-by-Example): recall 85.76% → 99.31%</li>
</ul>

<h3>Encrypted Traffic Detection via Statistical Randomness Testing <span class="cv-period">2026.07 — 2026.09</span></h3>
<p class="cv-role">Lead Researcher</p>
<ul>
<li>Demonstrated Shannon entropy + RNN cannot separate encrypted from naturally high-entropy data (overlap at 1e-5 granularity)</li>
<li>Introduced NIST SP 800-22 randomization tests as discriminative features; Block→Chunk→Replica three-tier architecture</li>
<li>17-dimensional feature selection; AUC 0.9998, Recall 99.6%, FPR 0.0045%; F1 0.928 → 0.975</li>
<li>NSGA-II multi-objective optimization for anomaly detection: 100% detection rate, 0% Generic false positive</li>
<li>Deployed to production; 1 patent disclosure</li>
</ul>

<h3>Video QA Data Engine for Multimodal LLM Fine-tuning <span class="cv-period">2026.04 — 2026.06</span></h3>
<p class="cv-role">Research Collaborator</p>
<ul>
<li>End-to-end pipeline for Qwen3.5-27B: 4 ad categories, 14 marketing comprehension sub-tasks</li>
<li>Dual-layer quality gating: rule validation + Gemini Pro LLM-as-a-Judge</li>
<li>39,513 training samples delivered; 134K API calls, 480M tokens; async with retry and checkpointing</li>
</ul>
</div>

<div class="cv-section">
<h2>Selected Projects</h2>

<h3>Vision-Based Tree Ring Identification System <span class="cv-period">2025.06 — 2025.09</span></h3>
<p class="cv-role">Project Lead · Guangzhou Institute of Forestry</p>
<ul>
<li>SAM3-Adapter + CLIP visual-semantic guidance for high-density tree ring segmentation</li>
<li>TensorRT FP16 deployment: 3× throughput, 60% memory reduction; accuracy &gt;95%</li>
<li>Exhibited at the National Ancient Tree Protection Week</li>
</ul>

<h3>LLM-Driven Risk Analysis for Safety Engineering <span class="cv-period">2025.03 — 2025.04</span></h3>
<p class="cv-role">LLM Lead</p>
<ul>
<li>Multi-modal RAG: risk factor extraction from accident reports → FRAM mapping → Bayesian Network generation</li>
<li>Core algorithms support a paper in <em>Reliability Engineering & System Safety</em> (SCI Q1)</li>
</ul>
</div>

<div class="cv-section">
<h2>Technical Skills</h2>
<ul>
<li><strong>AI Infra:</strong> vLLM, SGLang, CUDA, TensorRT, CANN/ACL, Nsight, msprof</li>
<li><strong>Frameworks:</strong> PyTorch, ONNX, Docker, Kubernetes</li>
<li><strong>ML/AI:</strong> Computer Vision, Multimodal Learning, LLM Serving, Data Engineering</li>
</ul>
</div>

<div class="cv-section">
<h2>Honors & Awards</h2>
<ul>
<li><strong>ASC 2025</strong> · Second Prize — World-wide University Supercomputing Competition</li>
<li><strong>National Encouragement Scholarship</strong></li>
<li><strong>University Scholarship</strong> · Merit Student</li>
</ul>
</div>
