# Emergent Coordination in Multi-Agent Language Models

**Authors**: Network Science Institute  
**Conference**: ICLR 2026  
**arXiv**: 2510.05174  
**Date**: January 30, 2026

---

## Abstract

We introduce an information-theoretic framework to test—in a purely data-driven way—whether multi-agent systems show signs of higher-order structure. This information decomposition lets us measure whether dynamical emergence is present in multi-agent LLM systems, localize it, and distinguish spurious temporal coupling from performance-relevant cross-agent synergy.

---

## Research Question

When are multi-agent LLM systems merely a collection of individual agents versus an integrated collective with higher-order structure?

---

## Methodology

### Information-Theoretic Framework

- **Partial Information Decomposition** of time-delayed mutual information (TDMI)
- Practical criterion and emergence capacity criterion
- Robust across emergence measures and entropy estimators

### Experimental Design

- Simple guessing game without direct agent communication
- Only minimal group-level feedback
- Three randomized interventions:
  1. Control condition
  2. Persona assignment
  3. Persona + "think about what other agents might do"

---

## Key Findings

### Experimental Results

| Condition | Result |
|-----------|--------|
| **Control** | Strong temporal synergy, but little coordinated alignment across agents |
| **Persona** | Stable identity-linked differentiation |
| **Persona + Theory of Mind** | Identity-linked differentiation + goal-directed complementarity |

### Core Insight

Multi-agent LLM systems can be **steered with prompt design** from mere aggregates to higher-order collectives.

---

## Collective Intelligence Principles

The observed patterns mirror well-established principles of collective intelligence in human groups:

> **Effective performance requires both alignment on shared objectives and complementary contributions across members.**

---

## Implications

1. **Prompt Engineering as Coordination Mechanism**: Simple prompt modifications can significantly alter collective behavior
2. **Theory of Mind Matters**: Encouraging agents to consider others' perspectives enhances coordination
3. **Identity Matters**: Assigning personas creates stable differentiation
4. **Higher-Order Structures are Achievable**: LLM collectives can exhibit true synergy, not just parallel execution

---

## Citation

```bibtex
@inproceedings{networkscience2026emergent,
  title={Emergent Coordination in Multi-Agent Language Models},
  author={Network Science Institute},
  booktitle={International Conference on Learning Representations (ICLR)},
  year={2026}
}
```

---

**Source**: https://www.networkscienceinstitute.org/publications/emergent-coordination-in-multi-agent-language-models
