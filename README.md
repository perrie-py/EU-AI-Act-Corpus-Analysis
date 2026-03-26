# EU AI Act: Corpus Analysis of Grammatical Voice and Social Actor Representation

A corpus-based critical discourse analysis (CDA) of the EU AI Act (2024), 
examining how grammatical voice encodes agency, accountability, and the 
representation of social actors in AI governance discourse.

## Research Questions

1. How are agency and answerability encoded in the EU AI Act through 
   grammatical voice?
2. How do grammatical choices function to background or obscure social 
   actors in the context of AI governance?

## Background

The EU AI Act (2024) is the first comprehensive binding regulatory 
framework for AI within the EU. As a legislative instrument designed to 
assign binding obligations to identifiable actors, its grammatical 
management of agency carries direct regulatory and accountability 
consequences. This study applies corpus-based CDA to examine how voice 
distribution and social actor representation construct accountability 
in an emerging regulatory framework.

## Corpus

- **Source:** Full English-language text of the EU AI Act (June 2024), 
  including footnotes
- **Size:** 104,308 tokens | 87,980 words | 2,015 sentences
- **Verbs identified:** 11,981 across 602 lemmas
- **Extracted using:** Sketch Engine concordance function

## Method

### Verb Selection
- Lemmas with a minimum of 70 concordance instances included, yielding 
  9 verb lemmas: *use, ensure, apply, facilitate, cover, affect, 
  provide, implement, require*
- 976 concordance lines analysed in total (670 active, 306 passive)
- Verbal adjectives, attributive verbs, and prepositional uses excluded

### Manual Coding
- Each concordance line coded for grammatical voice (active/passive)
- Social actors coded in pre-verbal (SAB) and post-verbal (SAA) positions
- Social actor categories derived inductively from the corpus
- Grammatical roles coded deductively using Van Leeuwen's (1996) 
  framework and Collins' (2005) smuggling analysis
- Categories: Agent, Subjected, Suppressed, Backgrounded, 
  Beneficiaries, Smuggled Patient

### Statistical Analysis
- Chi-squared tests on voice distribution across all 9 lemmas
- Standardised residuals to identify meaningful deviation 
  (threshold: ±2, following Agresti, 2007; Gries, 2009)
- Chi-squared tests on social actor distributions within 
  active-dominant lemmas (ensure, apply, facilitate) and 
  passive-dominant lemmas (use, cover)
- Proportional distribution of grammatical roles by social actor 
  across SAB and SAA positions

### Visualisation
- Voice frequency by lemma
- Social actor distributions (pre- and post-verbal) for each lemma, 
  split by voice condition
- Proportional grammatical role distribution by social actor using 
  `pivot_longer` and faceted bar charts

## Key Findings

- Voice distribution across lemmas is highly non-uniform (p < 2.2e-16)
- *Use* is passivised far more frequently than expected 
  (residuals: -7.09 active, +10.54 passive), systematically obscuring 
  human and institutional agents
- *Ensure*, *apply* and *facilitate* show strong active preference — 
  the Regulation itself is the dominant grammatical agent, 
  representing institutional abstraction of accountability
- AI systems dominate pre-verbal positions in passive constructions 
  of *use*, foregrounded syntactically but denied agency
- The public and civil society are near-absent from agent positions

## Theoretical Framework

`Corpus-based CDA` `Van Leeuwen (1996) social actor representation` 
`Collins (2005) smuggling analysis` `Halliday & Matthiessen (2014) 
transitivity` `Fairclough (2001)` `Baker (2006) corpus linguistics`

## Tools & Libraries

`R` `ggplot2` `dplyr` `tidyr` `Sketch Engine` 
`chi-squared analysis` `corpus linguistics` `critical discourse analysis`


## Ethics & Data Privacy
The corpus consists entirely of a publicly available legislative 
document (EU AI Act, 2024). No personal or participant data is included.

## Status
Dissertation in progress. Code will be uploaded upon completion 
and with academic approval.
