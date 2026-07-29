IBM SkillsBuild Learning Pathway Advisor
Live demo → https://cindymmy111-star.github.io/ibm-skillsbuild-recommender/

A rule-based recommendation tool that turns "which course should I take next?" into an explainable scoring problem. Built as an IBM-sponsored group project at the University of Bristol (MSc Business Analytics, Jan–May 2026).
Problem
IBM SkillsBuild offers a large catalogue of free courses, but students arriving with different degrees, skill levels and target roles have no structured way to decide where to start. Generic "most popular" lists ignore what a learner already knows and what their target job actually requires.
Approach
The tool collects a learner profile — degree programme, year of study, academic interests, target industry and job role, plus self-declared existing skills — and scores 12 IBM SkillsBuild courses across 6 criteria:

Criterion
What it captures
Skills-gap coverage
How much of the gap between current skills and target-role requirements the course closes
Role relevance
Alignment with the selected target job role
Subject relevance
Match against declared academic interests
Industry fit
Relevance to the chosen industry
Difficulty gating
Prevents recommending advanced courses before prerequisites are met
Sequencing
Orders surviving courses into a coherent learning pathway


Scores are combined into a ranked pathway, and every recommendation is returned with the reason it was selected, so the output can be audited rather than taken on trust. The interface also includes a progress dashboard, skill-coverage view, saved pathways and a feedback module.
My role — recommendation logic & data modelling
Designed the scoring model: defined the 6 criteria, the course–skill mapping, weightings and the difficulty-gating rules.
Implemented the rule engine in vanilla JavaScript (no framework, no build step, runs entirely client-side).
Wrote the technical documentation — system architecture, data-flow diagrams and scoring-algorithm specification — so the logic was reusable by the rest of the team and reviewable by the IBM client.
Coordinated with the client on requirements within a 6-person cross-functional team; received an "Excellent" contribution assessment for the project plan.
Tech
Vanilla JavaScript, HTML and CSS. Single self-contained file, deployed on GitHub Pages — no dependencies, no server, no API keys.
Repository
index.html    Complete application: UI, course data, scoring engine


IBM SkillsBuild 学习路径推荐系统（中文说明）
在线体验 → https://cindymmy111-star.github.io/ibm-skillsbuild-recommender/

布里斯托大学 × IBM 课程项目（商业分析硕士，2026.01–05），一个基于规则的课程推荐工具，把「下一门该学什么」变成可解释的评分问题。
问题
IBM SkillsBuild 有大量免费课程，但学生的专业背景、已有技能和目标岗位差异很大，靠「热门推荐」无法回答「我该从哪开始」。
方案
采集学习者画像（专业、年级、学术兴趣、目标行业与岗位、已有技能），对 12 门课程按 6 项维度打分：技能缺口覆盖度、岗位相关性、学科相关性、行业匹配度、难度门控、路径排序。最终输出排序后的学习路径，并给出每门课被选中的理由，使推荐结果可被审计而不是黑箱。界面另含进度看板、技能覆盖图、收藏路径与反馈模块。
我负责的部分
设计评分模型（6 项维度、课程—技能映射、权重与难度门控规则）；用原生 JavaScript 实现规则引擎；撰写系统架构、数据流图与评分算法技术文档；在 6 人跨职能团队中对接 IBM 客户需求，项目计划部分获评 "Excellent"。
技术
原生 JavaScript / HTML / CSS，单文件、无依赖、纯前端，部署在 GitHub Pages。
