# Interview Report Template

This file describes how to generate the final interview performance report.

## Scoring Rubric

### Per-Question Dimensions (1–5 scale)

| Score | Meaning |
|---|---|
| 5 | Exceptional — exceeded expectations, highly specific, structured |
| 4 | Good — covered main points, minor gaps |
| 3 | Adequate — answered but lacked depth or examples |
| 2 | Weak — partial answer, vague, missing key aspects |
| 1 | Poor — off-topic, incomplete, or no meaningful content |
| 0 | Skipped |

### Competency Areas (for radar chart)

Weight each answer into these 6 competency buckets:

1. **技术能力 / Technical Skills** — Depth of domain knowledge
2. **问题解决 / Problem Solving** — Analytical approach, tradeoffs
3. **沟通表达 / Communication** — Clarity, structure (STAR method)
4. **团队协作 / Collaboration** — Teamwork stories, conflict handling
5. **自我驱动 / Initiative** — Self-learning, proactiveness
6. **岗位匹配度 / Role Fit** — Alignment with JD requirements

### Overall Score Formula

```
Overall = (avg_technical × 0.35) + (avg_problem_solving × 0.25) + 
          (avg_communication × 0.20) + (avg_collaboration × 0.10) + 
          (avg_initiative × 0.05) + (avg_role_fit × 0.05)

Normalize to 100: Overall_100 = (Overall / 5) × 100
```

---

## Report HTML Template

When generating the report as a visual artifact, use this structure:

```html
<!-- Use the Visualizer tool to render this as an inline HTML widget -->
<!-- Color scheme: professional, clean, with role-appropriate accents -->

Structure:
- Header: Candidate name (if given) + Role + Date
- Hero: Big score number with color coding
  - 90-100: ⭐ gold
  - 75-89: 🟢 green  
  - 60-74: 🟡 yellow
  - below 60: 🔴 red
- Radar chart: 6-axis SVG spider chart with competency scores
- Question summary table: Q#, Topic, Score (colored dots), one-line note
- Two columns: Strengths (green checkmarks) | Improvements (orange arrows)
- Study recommendations: cards with topic + why + resources
- Verdict banner: full-width with readiness level
```

---

## Markdown Fallback Template

If Visualizer is not available, use this markdown structure:

```markdown
# 🎯 面试评估报告

**岗位**: [Role]  
**面试日期**: [Date]  
**总题数**: [N] 题

---

## 📊 综合得分: [XX]/100

> [Readiness verdict with emoji]

---

## 🕸️ 能力雷达

| 能力维度 | 得分 | 评级 |
|---|---|---|
| 技术能力 | X.X/5 | ⭐⭐⭐ |
| 问题解决 | X.X/5 | ⭐⭐⭐⭐ |
| 沟通表达 | X.X/5 | ⭐⭐ |
| 团队协作 | X.X/5 | ⭐⭐⭐ |
| 自我驱动 | X.X/5 | ⭐⭐⭐⭐ |
| 岗位匹配度 | X.X/5 | ⭐⭐⭐ |

---

## 📋 逐题得分

| # | 题目摘要 | 得分 | 简评 |
|---|---|---|---|
| 1 | ... | 4/5 | ... |
...

---

## ✅ 核心优势

1. **[Strength 1]**: ...
2. **[Strength 2]**: ...
3. **[Strength 3]**: ...

## 🔧 待提升方向

1. **[Gap 1]**: [具体建议]
2. **[Gap 2]**: [具体建议]
3. **[Gap 3]**: [具体建议]

---

## 📚 推荐学习方向

- **[Topic 1]**: 原因 + 建议资源
- **[Topic 2]**: 原因 + 建议资源
- **[Topic 3]**: 原因 + 建议资源

---

## 🏁 面试准备度

> [🔴 暂不建议投递 / 🟡 还需加强 / 🟢 可以投递 / ⭐ 表现出色]
> 
> [2-3 sentence personalized verdict]
```

---

## Report Generation Instructions

1. Tally all per-question scores from Phase 3
2. Map questions to competency areas (some questions count toward multiple areas)
3. Calculate weighted overall score
4. Identify top 3 strongest answers → extract themes as "strengths"
5. Identify bottom 3 weakest answers → extract gaps as "improvements"
6. Recommend 2–4 study topics based on the gaps (be specific: not just "study algorithms" but "practice dynamic programming — you struggled with the memoization question")
7. Render report using Visualizer if available, markdown otherwise
8. End with an encouraging but honest verdict
