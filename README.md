# Elevated Evidence Requirements in High Worriers: A Computational Replication of Tallis et al. (1991)


This project investigates how worry and broader transdiagnostic symptom dimensions influence decision-making under uncertainty. Using a visual search paradigm, the study applies Drift Diffusion Modelling (DDM) and Exploratory Factor Analysis (EFA) to decompose behavioural performance into latent cognitive mechanisms.

---

## Background

Decision-making under uncertainty is a core cognitive function, yet it is highly sensitive to affective and cognitive disturbances. Disruptions in uncertainty processing are linked to internalising conditions such as anxiety, depression, and obsessive–compulsive disorder.

Worry is a transdiagnostic cognitive style characterised by repetitive, uncontrollable thoughts about negative future events. Unlike physiological anxiety, worry involves sustained verbal–linguistic processing and difficulty disengaging from hypothetical threats. It has been proposed to influence decision-making by increasing the amount of evidence required before committing to a response—a construct known as **Elevated Evidence Requirement (EER)**.

Early behavioural work (e.g., Tallis et al., 1991) showed that high worriers are slower, particularly on target-absent trials requiring exhaustive search. However, these findings relied on aggregate measures (reaction time and accuracy), which cannot distinguish between underlying cognitive mechanisms such as:

- Increased decision caution  
- Reduced evidence accumulation efficiency  
- Impaired attentional control  
- Slower perceptual or motor processes  

---

## Computational Approach

This study applies the **Drift Diffusion Model (DDM)**, which decomposes decision-making into latent components:

- **Boundary separation (a):** decision threshold (response caution)  
- **Drift rate (v):** speed/quality of evidence accumulation  
- **Starting point (z):** response bias  
- **Non-decision time (t):** perceptual and motor processes  

Boundary separation provides a direct computational analogue of EER. If worry primarily affects decision strategy, it should manifest as increased boundary separation rather than reduced drift rate.

---

## Research Objectives

This study had two primary aims:

1. **Replication and extension**
   - Replicate Tallis et al. (1991) using a visual search paradigm  
   - Test whether worry-related slowing reflects increased boundary separation (EER) using DDM  

2. **Transdiagnostic modelling**
   - Examine whether latent symptom dimensions predict variation in DDM parameters  
   - Move beyond single-scale analyses using a transdiagnostic framework  

---

## Hypotheses

- High worriers will show **longer reaction times**, particularly on target-absent trials  
- Slower responses will be explained by **increased boundary separation**, not reduced drift rate  
- Any drift rate effects will be **condition-specific**, not global  
- **Non-decision time will not differ**, supporting a strategic (not peripheral) account  
- Latent symptom dimensions will predict DDM parameters:
  - Anxiety/compulsivity → increased boundary separation  
  - Depression → reduced drift rate  

---

## Methods

- **Participants:** N = 41 (post-exclusion)  
- **Task:** Visual letter-search paradigm (target present vs absent)  
- **Design:** Online administration  

### Measures
- PSWQ (worry)  
- WDQ (worry domains)  
- GAD-7 (anxiety)  
- PHQ-8 (depression)  
- OCI-R (obsessive–compulsive symptoms)  

### Analysis Pipeline

- Exploratory Factor Analysis (EFA) to derive latent symptom dimensions  
- Drift Diffusion Model (DDM) fitted to trial-level data  
- Linear Mixed-Effects Models (LME) to test:
  - Symptom effects  
  - Condition effects  
  - Interactions on DDM parameters  
