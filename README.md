# Experiment Plan – Scoping and Planning

## 1. Basic Identification

### Experiment Title
**Quality and Maintainability in Legacy Software: An Empirical Analysis of Refactorings on GitHub**

### ID / Code
**PUCM-ES-RES-2025-001**

### Document Version and Revision History
| Field | Value |
|-------|--------|
| Document Version | v1.1 |
| Revision History | - v1.0 — Initial draft (21 Nov 2025)<br>- v1.1 — Second delivery (25 Nov 2025) |

### Dates
| Field | Value |
|--------|--------|
| Creation Date | 21 November 2025 |
| Adding Sections | 25 November 2025 |

### Author
**Júlia Moreira** — Software Engineering Department  
Email: **moreira01092002@gmail.com**

### Principal Investigator
**Nascimento** (Study Lead)

### Related Work Overview
Prior studies indicate that:
- Refactoring improves structure but is risky in legacy systems.
- Refactoring React-based legacy systems reduces inconsistency but requires careful coordination.
- Refactorings often emerge during code review instead of planned technical-debt management.
- Large industrial repositories show complex refactoring branch dynamics.
- Multi-objective refactoring recommendation tools optimize decision-making.

These studies support the motivation behind this experiment.

---

# 2. Context and Problem

Legacy systems underpin critical operations across governments, finance, and enterprises.  
Despite this, they:
- are costly to maintain,
- rely on outdated technologies,
- accumulate technical debt,
- and frequently fail in modernization attempts.

Since 2010, **US \$35 trillion** has been spent on IT, **75%** of which went to maintenance.  
Among **US \$2.5 trillion** in modernization attempts, **\$720 billion** was wasted on failed efforts.

Refactoring is a lower-risk modernization technique but often fails due to:
- regressions,
- insufficient testing,
- complexity,
- metadata noise,
- and poor planning.

This study analyzes successful and unsuccessful refactorings on GitHub to identify patterns that differentiate them.

---

# 3. Goals and Questions (GQM Framework)

## 3.1 General Goal
Analyze refactoring activities in legacy software repositories to understand their impact on internal quality and maintainability within long-lived GitHub projects.

---

## 3.2 Specific Objectives

- **O1:** Identify structural/code-quality characteristics that differentiate successful from unsuccessful refactorings.  
- **O2:** Evaluate how refactorings affect maintainability indicators (complexity, smells, change-proneness).  
- **O3:** Analyze socio-technical factors associated with refactoring outcomes.  
- **O4:** Assess the reliability of metadata and automated refactoring-detection tools.

---

## 3.3 Research Questions

### O1 — Structural Characteristics
- Q1.1: What structural properties change before and after refactoring?  
- Q1.2: How often do unsuccessful refactorings introduce regressions?  
- Q1.3: Which refactoring types correlate with internal-quality improvements?

### O2 — Maintainability Impact
- Q2.1: How do complexity metrics evolve after refactoring?  
- Q2.2: Does refactoring reduce code smells?  
- Q2.3: What is the effect on change-proneness?

### O3 — Socio-technical Factors
- Q3.1: How does developer experience affect refactoring success?  
- Q3.2: What review patterns appear in successful vs unsuccessful refactorings?  
- Q3.3: Does development activity intensity increase defect likelihood?

### O4 — Metadata and Tool Reliability
- Q4.1: How accurate are automated refactoring-detection tools?  
- Q4.2: What false positives/negatives occur?  
- Q4.3: How reliable are commit messages and metadata?

---

# 3.4 GQM Table

| Goal | Questions | Metrics |
|------|-----------|---------|
| **O1 — Structural characteristics** | Q1.1 | M1, M2 |
| | Q1.2 | M3, M4 |
| | Q1.3 | M5, M6 |
| **O2 — Maintainability impact** | Q2.1 | M2, M7 |
| | Q2.2 | M8, M9 |
| | Q2.3 | M10, M11 |
| **O3 — Socio-technical factors** | Q3.1 | M12, M3 |
| | Q3.2 | M13, M14 |
| | Q3.3 | M11, M3 |
| **O4 — Tool reliability** | Q4.1 | M15, M16 |
| | Q4.2 | M15, M17 |
| | Q4.3 | M18, M19 |

---

# 3.5 Metrics Table

| Metric | Description | Unit |
|--------|-------------|-------|
| M1 | LOC variation | LOC |
| M2 | Cyclomatic complexity variation | Absolute |
| M3 | Post-refactoring defect count | Defects |
| M4 | Defect density | Def./KLOC |
| M5 | Refactoring type distribution | % |
| M6 | Static analysis quality score | 0–100 |
| M7 | Halstead complexity shift | Absolute |
| M8 | Code smell count | Count |
| M9 | Code duplication ratio | % |
| M10 | Change-proneness index | Changes/month |
| M11 | Churn volume | LOC |
| M12 | Developer experience level | Commits |
| M13 | Review comments count | Comments |
| M14 | Review participation size | People |
| M15 | Tool precision | % |
| M16 | Tool recall | % |
| M17 | False positive rate | % |
| M18 | Metadata consistency index | % |
| M19 | Commit-message accuracy | % |

---

# 4. Scope and Context

## 4.1 Scope (Included / Excluded)

### Included
- Mining GitHub repositories  
- Extracting refactoring data  
- Manual + automated validation  
- Commits, PRs, diffs, static-analysis reports  
- Legacy modules (≥ 5 years, ≥ 500 commits)

### Excluded
- Interviews with developers  
- Proprietary repositories  
- Runtime performance evaluation  
- Non-refactoring commits  

---

## 4.2 Study Context
- Open-source, distributed teams  
- Long-lived legacy codebases  
- Medium criticality  
- Mixed developer experience levels  

---

## 4.3 Assumptions
- Repository history is intact  
- Tools function reliably  
- Metadata accessible  
- Version-control best practices followed  

---

## 4.4 Constraints
- Limited time for manual validation  
- Dependence on tool accuracy  
- GitHub API rate limits  
- No contact with developers  

---

## 4.5 Limitations
- Limited generalization to industrial systems  
- Metadata noise  
- Mixed commits (refactoring + features)  
- Non-representative repository sample  

---

# 5. Stakeholders and Impact

## 5.1 Stakeholders
- Software engineers  
- Researchers  
- Open-source maintainers  
- Technical leaders  
- Tool developers  

---

## 5.2 Stakeholder Interests
- Engineers: Understanding refactoring risks  
- Researchers: Empirical evidence  
- Maintainers: Lower technical debt  
- Tech leads: Better modernization decisions  
- Tool developers: Real-world validation  

---

## 5.3 Impact
- Additional workload  
- Potential temporary delays  
- Better risk awareness  
- Improved modernization strategies  

---

# 6. Risks, Assumptions, and Success Criteria

## 6.1 High-Level Risks
- GitHub API failures  
- Tool inaccuracies  
- Metadata noise  
- Time limitations  
- Large dataset processing cost  

---

## 6.2 Success Criteria (Go / No-Go)
The experiment is successful if:
- ≥ 70% refactorings manually validated  
- Precision ≥ 75% and recall ≥ 70%  
- ≥ 80% of research questions answered  
- Clear distinction between successful and unsuccessful refactorings  

Otherwise → **No-Go**

---

## 6.3 Early Stop Criteria
- GitHub API unavailable  
- Tool malfunction  
- Repositories deleted/private  
- Insufficient computing/storage resources  
