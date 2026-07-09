**Case Analysis Form: Algorithmic Bias**

**1\. For EACH of the two cases, complete all four sections of the Case Analysis Form below.**

Both cases are analyzed below. Case 1: a commercial health-care risk-prediction algorithm (Obermeyer et al., Science, 2019). Case 2: the COMPAS criminal-risk algorithm (Angwin et al., ProPublica, 2016).

**2\. Section 1: What bias was identified and how was it measured? Include the specific magnitude of the finding (e.g., percentage gap, odds ratio).**

**Case 1:** Racial bias: at an equal risk score, Black patients are sicker. Measured by calibration. At the 97th percentile they had 26.3% more chronic conditions (4.8 vs 3.8; P<0.001); correcting it lifts the Black auto-enrolled share from 17.7% to 46.5%.

**Case 2:** Racial bias in how errors fall. Measured against two-year re-arrest (~7,000 defendants): false-positive rate 44.9% Black vs 23.5% White, nearly double; adjusted, Black defendants were 77% likelier to be rated high-risk for violent crime.

**3\. Section 2: Who was most harmed, and through what specific mechanism? Name the population and the institutional consequence.**

**Case 1:** Black patients. Because the score ranked by predicted cost, not illness, sicker Black patients were under-identified for high-risk care-management programs and denied the extra nursing and coordination they needed.

**Case 2:** Black defendants. The near-double false high-risk rate feeds bail, sentencing, and parole decisions, producing higher bond and longer incarceration for people who would not re-offend.

**4\. Section 3: Root cause classification - check all that apply from the bias taxonomy: \[ \] Historical bias \[ \] Representation bias \[ \] Measurement bias \[ \] Aggregation bias \[ \] Deployment bias. Provide one sentence of evidence for each checked category.**

**Case 1:** ☑ **Historical** ☐ Representation ☑ **Measurement** ☐ Aggregation ☐ Deployment

Historical: the system spends less on Black patients at equal need. Measurement: health-care cost is used as the proxy label for health need.

**Case 2:** ☑ **Historical** ☐ Representation ☑ **Measurement** ☐ Aggregation ☑ **Deployment**

Historical: arrest data encode disproportionate policing. Measurement: re-arrest proxies offending and questionnaire features proxy race. Deployment: built for rehabilitation needs, not the sentencing it is used in.

**5\. Section 4: Was remediation proposed or implemented? Evaluate its sufficiency: does it address the root cause or only the symptom?**

**Case 1:** Yes. The label was changed to a health-and-cost index, cutting excess conditions among Black patients by 84% (48,772 to 7,758). This targets the root cause (the proxy label), but it is partial and leaves the structural spending gap intact.

**Case 2:** No real fix. Northpointe disputed the findings and kept the formula proprietary. Responses were at most symptomatic (some judges defer less; Wisconsin paused scores in presentence reports); the root causes are untouched.

**6\. After both forms are complete, write a 100-word comparative synthesis: What do these two cases share as root causes, and what differs in the harm mechanism?**

Both algorithms share one root cause: measurement bias built on historical inequity. Each optimizes a convenient but distorted proxy for its true target. The health tool predicts cost as a stand-in for need; COMPAS predicts re-arrest as a stand-in for crime. Both proxies absorb structural racism (unequal medical spending; disproportionate policing), and neither model uses race directly, yet both reproduce it. The harm mechanisms diverge. The health algorithm harms by omission: sicker Black patients are under-identified and denied care. COMPAS harms by commission: Black defendants are over-flagged, producing harsher bail, sentencing, and parole. One withholds a benefit; the other imposes a penalty.