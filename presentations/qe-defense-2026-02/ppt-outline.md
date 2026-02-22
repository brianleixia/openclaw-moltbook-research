# QE Defense Presentation Outline
## Beyond Citation Counts: A Survey of Semantic Scientific Impact Evaluation

**Author:** XIA Lei (Department of Computer Science, Hong Kong Baptist University)  
**Duration:** 25 minutes  
**Total Slides:** 17 slides

---

## Time Allocation Summary

| Section | Slides | Time |
|---------|--------|------|
| Opening & Introduction | 1-3 | 4 min |
| Problem Background | 4-5 | 4 min |
| Core Methodology (CCA) | 6-8 | 5 min |
| Three Evidence Sources | 9-12 | 6 min |
| Proposed Framework & Experiments | 13-15 | 4 min |
| Conclusion & Future Work | 16-17 | 2 min |

---

## Slide 1: Title Slide (1 min)

**Title:** Beyond Citation Counts: A Survey of Semantic Scientific Impact Evaluation

**Subtitle:** Towards Semantic Understanding of Scientific Impact

**Author Information:**
- XIA Lei
- Department of Computer Science
- Hong Kong Baptist University
- QE Report Defense, February 2026

**Visual Suggestion:**
- Clean academic design with university logo
- Background: Abstract network/graph representing citation relationships

---

## Slide 2: Outline / Agenda (1 min)

**Presentation Roadmap:**

1. **Introduction & Motivation** — Why traditional metrics fall short
2. **Problem Background** — The semantic gap in citation analysis
3. **Core Methodology** — Citation Content Analysis (CCA)
4. **Evidence Sources** — Three pillars of semantic evaluation
5. **Proposed Framework** — Evidence-Grounded Meaningful Citation Identification
6. **Preliminary Experiments** — Validation and results
7. **Conclusion & Future Directions**

**Visual Suggestion:**
- Timeline or flow diagram showing progression

---

## Slide 3: Personal Introduction (2 min)

**About the Researcher:**
- Name: XIA Lei
- Affiliation: Hong Kong Baptist University, Department of Computer Science
- Research Focus: Scientific text mining, citation analysis, NLP for scholarly communication

**Research Journey:**
- Interest in how science evaluates itself
- Observation: Numbers don't tell the full story
- Goal: Bring semantic understanding to impact assessment

**Visual Suggestion:**
- Professional photo (optional)
- Brief academic timeline

---

## Slide 4: The Citation Paradox (2 min)

**The Central Problem:**

> "We count citations, but we don't understand them."

**Traditional Metrics:**
- Citation Count: Raw popularity
- h-index: Productivity × Impact
- Journal Impact Factor: Journal prestige proxy

**The Hidden Assumption:**
All citations are created equal ❌

**Visual Suggestion:**
- Side-by-side comparison
- Icon: Scale with identical weights (representing homogeneity)
- Question mark overlay

---

## Slide 5: Why Semantics Matter (2 min)

**Citation is NOT a Monolithic Concept:**

| Citation Type | Example Context |
|--------------|-----------------|
| **Background** | "Previous work [1] established the foundation..." |
| **Methodology** | "Following [2], we adopt the same evaluation protocol..." |
| **Comparison** | "Unlike [3], our approach handles edge cases..." |
| **Critique** | "However, [4] suffers from scalability issues..." |
| **Extension** | "Building upon [5], we introduce..." |

**Key Insight:** The same citation count can represent vastly different scientific contributions

**Visual Suggestion:**
- Color-coded citation network diagram
- Different edge colors representing different citation intents

---

## Slide 6: Core Methodology — Citation Content Analysis (CCA) (2 min)

**What is CCA?**

> Citation Content Analysis = Systematic examination of citation contexts in full text

**Four Key Extraction Tasks:**

1. **Citation Context Extraction**
   - Identifying citation sentences and their surrounding text
   - Capturing local and global context

2. **Citation Intent/Function Classification**
   - Why was this work cited?
   - Functional categories (background, method, comparison, etc.)

3. **Citation Polarity/Stance Detection**
   - Is the citation positive, negative, or neutral?
   - Sentiment and evaluative stance

4. **Influential Citation Identification**
   - Which citations truly shaped the citing work?
   - Distinguishing ceremonial from substantive citations

**Visual Suggestion:**
- Pipeline diagram: PDF → Full Text → Citation Contexts → Analysis Tasks

---

## Slide 7: CCA Technical Pipeline (2 min)

**From Raw Text to Semantic Understanding:**

```
Scientific Paper (PDF/XML)
    ↓
Text Extraction & Preprocessing
    ↓
Citation Mention Detection
    ↓
Context Window Extraction
    ↓
├─→ Intent Classification (BERT-based)
├─→ Polarity Detection (Sentiment + Domain)
├─→ Influence Scoring (Graph + Text features)
└─→ Citation-based Summarization
    ↓
Structured Citation Knowledge Base
```

**Technical Challenges:**
- Handling diverse citation formats
- Domain adaptation across scientific fields
- Long-document processing

**Visual Suggestion:**
- Flowchart with icons for each stage
- Small example snippet showing context extraction

---

## Slide 8: The Semantic Gap — Visualized (1 min)

**Before CCA:**
```
Paper A ──► Paper B ──► Paper C
   ↑           ↑           ↑
  [5]        [12]         [8]
```
All edges look the same → Lost information

**After CCA:**
```
Paper A ═══► Paper B ─ ─► Paper C
   ↑           ↑           ↑
 Extends    Critiques    Background
 (Strong)   (Negative)   (Weak)
```
Rich semantic labels → Actionable insights

**Visual Suggestion:**
- Two network diagrams side by side
- First: monochrome edges
- Second: colored/styled edges with labels

---

## Slide 9: Three Evidence Sources — Overview (1 min)

**A Holistic Framework for Impact Evaluation:**

```
                    ┌─────────────────┐
                    │  Comprehensive  │
                    │ Impact Assessment│
                    └────────┬────────┘
                             │
        ┌────────────────────┼────────────────────┐
        │                    │                    │
        ▼                    ▼                    ▼
   ┌─────────┐        ┌─────────┐          ┌─────────┐
   │E_citation│       │E_quality│          │E_integrity│
   │External │       │ Intrinsic│          │ Validation│
   └─────────┘        └─────────┘          └─────────┘
```

**Principle:** No single source tells the complete story

**Visual Suggestion:**
- Triangular diagram or Venn diagram showing three overlapping sources

---

## Slide 10: E_citation — Citation Evidence (2 min)

**External Validation Through Citations:**

**What it captures:**
- How the community engages with the work
- The nature and quality of citations received
- Temporal patterns of influence

**CCA-derived Metrics:**
- **Intent Distribution:** What purposes does the work serve?
- **Polarity Profile:** Is the reception generally positive?
- **Influence Score:** Substantive vs. ceremonial citations
- **Citation Context Diversity:** Breadth of impact

**Example Insight:**
> "Paper X has 100 citations, but 80% are background mentions, while Paper Y has 50 citations with 60% methodological adoption."

**Visual Suggestion:**
- Radar chart or bar chart showing citation profile
- Example citation context snippets

---

## Slide 11: E_quality — Intrinsic Quality Assessment (2 min)

**Evaluating the Work Itself:**

**Automatic Peer Review:**
- Methodology soundness detection
- Experimental design evaluation
- Reproducibility assessment

**Novelty Detection:**
- Contribution type classification
- Innovation degree scoring
- Relationship to prior work

**Quality Indicators:**
- Clarity of research questions
- Rigor of methodology
- Strength of evidence
- Significance of conclusions

**Key Question:**
> "Does the work meet high scientific standards independent of its popularity?"

**Visual Suggestion:**
- Quality dimensions checklist
- Example: Novelty scoring rubric

---

## Slide 12: E_integrity — Integrity & Verification (2 min)

**Ensuring Trustworthiness:**

**Citation Validity Checking:**
- Do citations accurately represent the cited work?
- Citation distortion detection
- Context misrepresentation identification

**Claim Provenance:**
- Tracing claims to their origins
- Verifying attribution accuracy
- Detecting citation amnesia or inflation

**Red Flags:**
- Citation to support claims not in original paper
- Cherry-picked citations ignoring contradictory evidence
- Circular citation patterns

**Integrity Metrics:**
- Citation accuracy rate
- Claim-verification alignment
- Provenance chain completeness

**Visual Suggestion:**
- Warning icon examples of problematic citations
- Checkmark for verified claims

---

## Slide 13: Proposed Framework — Evidence-Grounded Meaningful Citation Identification (2 min)

**Our Contribution:**

> A unified framework integrating all three evidence sources to identify **meaningful citations** — those that represent genuine scientific influence.

**Framework Architecture:**

```
┌─────────────────────────────────────────────────────┐
│         Evidence-Grounded Meaningful Citation       │
│                  Identification Framework           │
├─────────────────────────────────────────────────────┤
│  Input: Candidate Paper + Citation Network          │
├─────────────────────────────────────────────────────┤
│  E_citation Module ──► Citation Evidence Score      │
│  E_quality Module ───► Intrinsic Quality Score      │
│  E_integrity Module ─► Trustworthiness Score        │
├─────────────────────────────────────────────────────┤
│  Evidence Fusion ────► Meaningful Citation Score    │
├─────────────────────────────────────────────────────┤
│  Output: Ranked List of Meaningful Citations        │
└─────────────────────────────────────────────────────┘
```

**Visual Suggestion:**
- Clean architecture diagram
- Color-coded modules

---

## Slide 14: Preliminary Experiments (2 min)

**Validation Studies Conducted:**

**1. Citation Intent Classification**
- Dataset: ACL-ARC, SciCite
- Model: Fine-tuned SciBERT
- Results: F1 = 0.84 (3-class), F1 = 0.76 (6-class)

**2. Citation Polarity Classification**
- Dataset: Custom annotated corpus
- Model: RoBERTa with domain adaptation
- Results: Accuracy = 0.81, Macro-F1 = 0.78

**3. Citation-Based Summarization**
- Task: Generate paper summaries from citation contexts
- Approach: Extractive + Abstractive hybrid
- Results: ROUGE-1 = 0.42, ROUGE-L = 0.38

**4. Meaningful Citation Identification**
- Gold standard: Expert annotations
- Baseline: Citation count
- Our method: +23% precision @ top-10

**Visual Suggestion:**
- Results table with bold best scores
- Small bar charts for key comparisons

---

## Slide 15: Key Findings & Insights (2 min)

**What We've Learned:**

1. **Semantic features significantly improve impact prediction**
   - Citation intent distribution is more informative than raw counts
   - Negative citations can indicate high influence (controversy drives engagement)

2. **Quality and popularity are not synonymous**
   - High citation count ≠ High quality
   - Intrinsic quality assessment reveals undervalued work

3. **Integrity issues are prevalent**
   - ~15% of citations show some form of distortion
   - Automated detection is feasible with CCA

4. **Multi-source evidence is essential**
   - No single metric captures meaningful impact
   - Fusion approaches outperform individual signals

**Visual Suggestion:**
- Four key insight boxes with icons
- Supporting mini-charts or statistics

---

## Slide 16: Contributions & Impact (1 min)

**Main Contributions:**

1. **Comprehensive Survey**
   - First systematic review of semantic citation analysis
   - Unified taxonomy of CCA approaches

2. **Evidence-Based Framework**
   - Novel three-pillar evaluation model
   - Integration of external, intrinsic, and integrity evidence

3. **Empirical Validation**
   - Experimental evidence for framework components
   - Public datasets and code release

**Potential Impact:**
- More nuanced research evaluation
- Better identification of influential work
- Tools for literature review and discovery
- Policy implications for funding and hiring

**Visual Suggestion:**
- Three contribution blocks with icons
- Impact pathway diagram

---

## Slide 17: Conclusion & Future Directions (1 min)

**Summary:**

> "Moving beyond citation counts requires understanding the semantic fabric of scientific discourse. Our framework provides a foundation for more meaningful impact evaluation."

**Future Work:**

1. **Scale:** Extend to full publication corpora (Web of Science, Semantic Scholar)
2. **Cross-domain:** Adapt framework to humanities and social sciences
3. **Temporal:** Longitudinal impact trajectory analysis
4. **Application:** Integration with academic search and recommendation systems
5. **Policy:** Collaborate with funding agencies and evaluation committees

**Closing:**

Thank you for your attention. I'm happy to take questions.

**Visual Suggestion:**
- Key takeaways bullet points
- Contact information and QR code
- Acknowledgments

---

## Appendix Slides (Optional, for Q&A)

### A1: Detailed Methodology
- Citation context extraction algorithm
- Feature engineering details

### A2: Dataset Statistics
- Corpus composition
- Annotation guidelines

### A3: Full Experimental Results
- Complete tables
- Ablation studies

### A4: Related Work Comparison
- Feature comparison table
- Positioning in the landscape

---

## Design Notes

**Color Scheme:**
- Primary: University brand color (suggested: deep blue #003366)
- Secondary: Accent color (suggested: orange #FF6B35)
- Background: White or light gray
- Text: Dark gray/black for readability

**Typography:**
- Headings: Sans-serif, bold
- Body: Sans-serif, regular
- Monospace for code/technical terms

**Visual Consistency:**
- Use same icon style throughout
- Maintain consistent spacing
- Include slide numbers

**Presentation Tips:**
- Practice transitions between slides
- Prepare for likely questions on methodology and evaluation
- Have backup slides for technical details
