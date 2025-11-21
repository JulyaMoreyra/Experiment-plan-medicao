# Experiment Plan – Scoping and Planning

## Basic Identification

### **Experiment Title**
**Quality and Maintainability in Legacy Software: An Empirical Analysis of Refactorings on GitHub**

### **ID / Code**
**Experiment ID:** PUCM-ES-RES-2025-001

### **Document Version and Revision History**

| Field | Value |
|-------|--------|
| Document Version | v1.0 |
| Revision History | - v1.0 — Initial draft (21 Nov 2025) — Júlia Moreira |

### **Dates (creation, last update)**

| Field | Value |
|-------|--------|
| Creation Date | 21 November 2025 |

### **Author (name, department, contact)**

- **Author 1:** Júlia Moreira, Software Engineering Department  
  Email: *moreira01092002@gmail.com*

### **Principal Investigator / Experiment Owner**

- **PI / Owner:** Nascimento (Principal Investigator / Study Lead)

### **Related Project / Product / Initiative**

Recent research has explored challenges and opportunities in refactoring legacy software systems, offering empirical insights relevant to this study.

Yanakiev et al. (2025) describe the application of SOLID principles in legacy systems and show improvements in structural complexity and maintainability.  
Ferreira et al. (2024) explore refactoring in React applications and highlight technical debt issues caused by framework evolution.  
Coelho et al. (2025) analyze refactorings triggered during code reviews, emphasizing their socio-technical nature.  
Alomar et al. (2025) investigate refactoring branches in the Qt ecosystem, identifying risks and integration challenges.  
Chen et al. (2024) propose MORCoRA, a multi-objective refactoring recommender considering reviewer availability.

These studies provide a solid foundation for understanding refactoring in legacy systems.

---

# Context and Problem

Legacy software systems remain essential in governments, financial institutions, and enterprises. Despite their importance, modernization imposes huge financial and organizational burdens. According to Charette (IEEE Spectrum), since 2010 organizations have spent **US\$35 trillion** on IT, with **75%** devoted to maintaining existing systems.

Additionally, approximately **US\$720 billion** has been wasted on failed modernization projects, including unsuccessful refactoring and rewrite attempts.

Legacy systems rely on outdated technologies, unsupported hardware, and decades of accumulated architectural erosion. This makes modernization risky and expensive.

In 2019, nearly **80%** of the U.S. government’s IT budget** was spent just to keep legacy systems running.

Refactoring is positioned as a lower-risk alternative to rewriting entire systems, but its success is inconsistent and often lacks empirical grounding. This motivates the present study: to analyze real refactoring efforts in open-source repositories and identify what differentiates successful from unsuccessful attempts.

---

## Problem / Opportunity Description

Legacy systems, despite their critical role, suffer from low performance, poor maintainability, and high structural complexity. Refactoring is a common strategy to improve internal quality while preserving behavior.

However, in practice many refactorings **fail**. Symptoms include:

- increased defect rates  
- longer development cycles  
- rising maintenance costs  
- limited adherence to best practices  

Organizations invest heavily in modernization, but many efforts fail due to poor planning, absence of metrics, and insufficient understanding of refactoring impact.

Thus, this study presents an opportunity to **empirically analyze successful and unsuccessful refactorings** in GitHub repositories to extract actionable patterns and risk indicators.

---

## Organizational and Technical Context

Refactoring legacy systems happens under strong constraints:

### **Organizational**
- high dependency on stability and availability  
- regulatory demands  
- budget limitations  
- pressure for continuous delivery  

### **Technical**
- outdated languages and frameworks  
- monolithic architectures  
- low test coverage  
- insufficient documentation  
- tightly coupled modules  
- loss of institutional knowledge  

These factors reinforce the need for empirical analysis in environments where repository evolution can be observed.

---

## Prior Work and Evidence (Internal and External)

Studies such as Yanakiev et al. (2025) and Ferreira et al. (2024) show that incremental refactoring often improves maintainability, though outcomes differ depending on context.

Coelho et al. (2025) highlight the socio-technical role of code reviews in triggering refactorings.  
Alomar et al. (2025) show that poorly structured refactoring branches can lead to regressions.  
Chen et al. (2024) show that reviewer availability affects refactoring prioritization.

Industry reports show billions wasted in failed modernization projects, reinforcing the need for better understanding of refactoring dynamics.

---

## Essential Theoretical and Empirical Background

This study is grounded in:

### **Software Maintenance and Evolution Theory**
- Lehman's Laws: systems degrade unless continuously evolved.

### **Refactoring Theory**
- Fowler (2018) and Mens & Tourwé (2004): refactoring is a behavior-preserving structural improvement.

### **Technical Debt**
- High technical debt increases defects and long-term costs.  
- Legacy systems accumulate architectural debt and code smells.

### **Empirical Software Engineering**
- Repository mining  
- Automated refactoring tools  
- Multi-objective decision support  

These theories support the methodology of examining real refactorings in public GitHub repositories.

