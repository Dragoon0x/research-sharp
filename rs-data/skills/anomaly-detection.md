---
id: anomaly-detection
name: Anomaly Detection
domain: rs-data
version: 1.0.0
---

# Anomaly Detection

**Purpose:** Master anomaly detection as a research discipline — the specific methods, frameworks, and judgment calls that produce reliable insights and confident decisions.

Anomaly Detection is where research becomes craft. The difference between a study that produces "interesting findings" and one that changes a $10M product decision is the practitioner's skill in designing the approach, executing the method, and synthesizing the results into action.

## The Core Framework

Effective anomaly detection requires three capabilities working together:

**Capability 1 — Research Design.** The ability to translate a business question into a researchable question, select the appropriate method, define the sample, and anticipate pitfalls. Poor design produces unreliable data regardless of execution quality. Design should take 20-30% of total study time — the highest-leverage investment in quality.

**Capability 2 — Rigorous Execution.** The ability to collect data without introducing bias, manage participants effectively, handle unexpected situations, and maintain quality throughout. Execution discipline means: following the protocol, documenting deviations, and catching problems early enough to correct them.

**Capability 3 — Actionable Synthesis.** The ability to transform raw data into structured insights that stakeholders act on. Synthesis is the rarest research skill — most practitioners collect well but struggle to distill data into the 3-5 findings that matter most.

## Advanced Techniques

### The Quality Assurance Framework

**Pre-study checklist.** Is the research question specific and answerable? Is the method appropriate? Is the sample representative and adequately sized? Has the protocol been pilot-tested? Are analysis plans defined before data collection? A study that fails pre-study review should not proceed — bad research costs more than no research.

**During-study monitoring.** Are participants engaging genuinely? Is data quality consistent? Are patterns emerging that suggest protocol problems? Is the sample balancing across important dimensions? Mid-study corrections are legitimate — catching a problem after 5 sessions is better than discovering it after 20.

**Post-study validation.** Do findings triangulate with other data sources? Are conclusions supported by sufficient evidence? Could an alternative explanation account for the same data? Have you stress-tested your interpretation by seeking disconfirming evidence?

### The Measurement Framework
Track research effectiveness across three dimensions:

**Methodological quality.** Was the study designed and executed rigorously? Did it follow best practices? Were biases identified and mitigated?

**Insight quality.** Are findings specific, evidence-based, and actionable? Do they reveal something the team didn't already know? Are they relevant to the decision they were designed to inform?

**Impact quality.** Did the research change a decision? Did the team act on findings? Can you trace a product or business outcome to the research? Impact is the ultimate measure — research that doesn't influence decisions has zero business value.


## The Data Analysis Operating System

### The Analysis Framework Selection
**Descriptive (what happened?).** Averages, distributions, trends, counts. Dashboards, summary stats. Most common and most often confused with insight — describing what happened is not explaining why.

**Diagnostic (why?).** Correlation, segmentation, cohort analysis, funnel analysis. Key discipline: correlation is not causation. "Onboarding completers retain better" might mean onboarding causes retention OR motivated users do both.

**Predictive (what will happen?).** Regression, time series, ML models. Critical caveat: predictions assume the future resembles the past.

**Prescriptive (what should we do?).** A/B test analysis, optimization models. Choose between specific options with measurable trade-offs.

### The Statistical Literacy Essentials
**Sample size and power.** Calculate before collecting. Consider: effect size, confidence level (95%), power (80%). Underpowered studies waste time and money.

**Confidence intervals > p-values.** P-values: is the effect real? CIs: how big is the effect? A significant 0.1% improvement is real but meaningless. The CI reveals this.

**Simpson's Paradox.** A trend in subgroups can reverse when combined. Treatment A better in men AND women but B better overall (because severe cases got A). Always segment before concluding.

**Survivorship bias.** Analyzing only what you can see while ignoring what you can't. Studying only successful startups misses the failed ones with identical patterns.

### The Experimentation Rigor Framework
**Tier 1 — Minimum viable (days).** Before/after, basic metrics. Low-risk, reversible changes.

**Tier 2 — Standard A/B (1-2 weeks).** 50/50 split. 1,000+ conversions per variant. 95% confidence. Pre-registered metric.

**Tier 3 — Full experiment (2-4 weeks).** Pre-registered hypothesis + primary metric + guardrails. Power analysis. Segment analysis post-experiment.

**Tier 4 — Holdout (1-3 months).** 5-10% holdout from all changes. Measures cumulative improvement.

### Case Study: Netflix Data-Driven Decision Making
~250 A/B tests running constantly. Artwork personalization per viewer through artwork A/B tests. Content investment driven by completion rates and re-watch rates, not reviews. 2-minute rule: if viewers don't engage in 2 min, they won't finish. Data infrastructure investment enables decision-making advantages that compound.

### The Dashboard Design Framework
**Row 1 (the answer).** North Star metric, this week vs last week vs same week last year. 3 seconds to understand health.

**Row 2 (the why).** Input metrics that explain changes. Which input drove the decline?

**Row 3 (the how).** Experiment results and channel performance.

**Row 4 (the health).** Guardrails: revenue, NPS, support tickets, error rates.

Everything else in secondary dashboards. Primary = 4 rows, no scrolling.

### The Data Visualization Decision Framework
**Comparison** -> Bar chart. Never pie charts for comparison. **Trend** -> Line chart. **Composition** -> Stacked bar or treemap. Pie only for 2-5 segments. **Distribution** -> Histogram or box plot. **Relationship** -> Scatter plot.

**The annotation rule.** Every chart self-explanatory without walkthrough: descriptive title, axis labels with units, data labels on key points, annotations on anomalies.

### The Cohort Analysis Masterclass
**Define the cohort.** Usually signup week/month. But behavioral cohorts more revealing: activated vs not, paid vs organic.

**Choose the metric.** Retention rate, engagement depth, or revenue per cohort.

**Read the chart.** Newer cohorts better or worse? Where does each flatten? Inflection points suggest specific problems (day 3 drop = onboarding failure).

**Act.** The chart tells WHERE. Qualitative research tells WHY. Combine.

### The Incrementality Testing Method
**Step 1.** Identify channel/tactic to test.
**Step 2.** Create 10-20% holdout that doesn't receive the treatment.
**Step 3.** Measure exposed vs holdout conversion rates. The difference = incremental impact.
**Step 4.** Calculate true ROI from incremental conversions, not attributed conversions.

Frequently reveals: branded search, retargeting, and email are less incremental than attribution suggests. Content and brand are more incremental.





### The Data Quality Framework
Bad data produces confident wrong answers. Verify before analyzing:

**Completeness.** Are there missing values? How many? Are they random or systematic? If 30% of a column is missing, the column may not be usable. If missing values cluster in a specific segment, analyzing that segment is unreliable.

**Consistency.** Are the same things measured the same way? If "active user" was defined as "logged in within 30 days" in Q1 and "performed an action within 7 days" in Q2, the metrics aren't comparable. Document every definition change.

**Accuracy.** Does the data reflect reality? Cross-validate: does the revenue in the analytics tool match the revenue in the accounting system? Does the user count in the dashboard match the count in the database? Discrepancies reveal tracking errors.

**Timeliness.** Is the data current enough for the decision? A market sizing based on 3-year-old data may be directionally correct but off by 30-50% in fast-moving markets. Date every data source and flag anything older than 12 months for validation.

**The cleaning protocol.** Before any analysis: (1) check for duplicates, (2) verify data types (dates as dates, numbers as numbers), (3) identify and handle outliers (investigate — don't just remove), (4) validate against external sources, (5) document every cleaning decision. The cleaning log is part of the analysis — it enables reproducibility and reveals data quality patterns.

### The Regression Analysis Quick Guide
The most useful statistical technique for business research:

**When to use.** You want to understand the relationship between one outcome variable and one or more predictor variables. "Does company size predict deal size?" "Which features predict retention?" "What factors predict NPS?"

**Interpreting coefficients.** Each coefficient = the expected change in the outcome for a one-unit change in the predictor, holding all other predictors constant. A coefficient of 5.3 on "team size" in a deal size regression means: each additional person on the buying team is associated with $5.3K larger deals, all else being equal.

**R-squared.** The percentage of outcome variation explained by the model. R² = 0.4 means the model explains 40% of the variation. In social science research, 0.3-0.5 is typical. Below 0.1 = the predictors barely matter. Above 0.7 = strong model.

**The caution.** Regression shows association, not causation. "Companies that use our premium plan retain longer" might mean premium causes retention, or it might mean companies that were going to retain anyway chose premium. Causation requires experimentation, not regression.




### The Analysis Documentation Standard
Every analysis should be reproducible by someone else:

**The analysis log.** For every analysis: (1) the question being answered, (2) the data sources used (with dates and version), (3) the cleaning steps applied (with justification), (4) the analytical method (with parameters), (5) the results (with confidence intervals), (6) the interpretation (with caveats). If you were hit by a bus, could a colleague reproduce your analysis from the log? If not, the documentation is insufficient.

**The version control discipline.** For code-based analysis: use git. For spreadsheet analysis: save versioned copies at each major step. For BI-based analysis: document the filters, segments, and date ranges. Analysis without version control is a black box that nobody can verify or build upon.

### The Segmentation Analysis Deep Dive
Segmentation is the most strategically valuable analysis:

**RFM segmentation.** Recency (when did they last engage?), Frequency (how often do they engage?), Monetary (how much do they spend?). Score each dimension 1-5. Group into segments: Champions (555), Loyal (X4X-X5X), At Risk (decreasing R), Hibernating (low R, any F/M). Each segment gets a different strategy.

**Behavioral segmentation.** Cluster users by what they DO, not who they ARE. Feature usage patterns, engagement frequency, content consumption patterns, session depth. k-means clustering on behavioral data typically reveals 3-5 natural segments that map to different product needs.

**Predictive segmentation.** Which current behaviors predict future outcomes (churn, expansion, referral)? Build a simple logistic regression: outcome = f(behaviors). The highest-weight behaviors become the early warning signals and intervention triggers.




### The Research Presentation Mastery Framework
Research that doesn't persuade is research that doesn't matter:

**The narrative arc.** Every research presentation follows: Context (why we did this research) -> Key Findings (the 3-5 insights that matter) -> Implications (what the findings mean for our decisions) -> Recommendations (what we should do next). This arc takes 15-20 minutes. Everything else goes in the appendix.

**The evidence hierarchy in presentations.** Most persuasive: video clip of a user struggling (5 seconds of video beats 50 slides). Then: specific quotes with attribution. Then: data visualizations with clear annotations. Least persuasive: bullet points of summary findings. Lead with the most persuasive evidence.

**The "so what" test.** For every slide, ask: "So what? Why does this matter for the decision we're making?" If you can't answer in one sentence, the slide doesn't belong in the main presentation.

**The stakeholder-specific adaptation.** Executives: lead with the recommendation, support with evidence. Product managers: lead with user insights, connect to product implications. Engineers: lead with user behavior patterns, connect to technical requirements. Designers: lead with user emotion and context, connect to design direction. Same findings, different emphasis.

### The Mixed Methods Integration Framework
The most powerful research combines qualitative and quantitative:

**Sequential explanatory design.** Start quantitative (survey, analytics) -> identify patterns -> follow with qualitative (interviews) to explain the patterns. "Analytics show 40% drop-off at step 3. Interviews reveal why: users don't understand why we need their company size."

**Sequential exploratory design.** Start qualitative (interviews) -> identify themes -> follow with quantitative (survey) to measure prevalence. "Interviews surfaced 3 key pain points. Survey of 500 users confirms pain point #2 is the most widespread (72% affected)."

**Concurrent triangulation.** Run qualitative and quantitative simultaneously on the same research question. Compare findings. Agreement = confidence. Disagreement = investigate further (usually reveals segment differences).

**The integration rule.** Never report qualitative and quantitative findings separately. Integrate: "Analytics show X [quant]. Users explain that this happens because Y [qual]. The combination suggests we should Z [recommendation]." The integration is where the research value lives.

### The Research Ethics in Practice
Beyond institutional guidelines — the practical ethics that matter:

**The do-no-harm principle.** Research should never leave participants worse off than before. If a study reveals that a participant is in a harmful situation (abusive relationship, dangerous working conditions, health risk), have a protocol: how to provide resources without overstepping the researcher role.

**The honest representation principle.** Never cherry-pick quotes or data to support a predetermined conclusion. If the evidence contradicts the hypothesis, report that honestly. Selective reporting is the most common ethical failure in business research — and the one with the longest-lasting damage to the research function's credibility.

**The participant dignity principle.** Participants are not "subjects" or "data points." They're people who are sharing their time and experiences. Use respectful language in reports. Never mock participant behavior (even privately). Frame struggles as design failures, not user failures.

**The confidentiality principle.** What participants share in research sessions is confidential. Anonymize in reports. Never share identifiable information without explicit consent. Never use research recordings for purposes beyond what was consented to. Protect participant identity as you would protect your own.

### The Research Tool Evaluation Framework
Choosing the right tools for the research stack:

**Recording and note-taking.** Requirements: reliable recording (audio + video + screen), automatic transcription, searchable transcripts, highlight and tag capability. Options: Lookback (best for UX research), Dovetail (best for analysis integration), Zoom (most accessible, least specialized).

**Analysis and synthesis.** Requirements: tagging/coding, theme generation, search across studies, collaboration. Options: Dovetail (purpose-built for research), EnjoyHQ (strong repository), Airtable (flexible, lower cost), Miro (for visual synthesis).

**Survey.** Requirements: skip logic, piping, randomization, analytics, export. Options: Qualtrics (most powerful, most expensive), Typeform (best UX, good for simple surveys), SurveyMonkey (middle ground), Google Forms (free, limited).

**Recruitment.** Requirements: screener management, scheduling, incentive distribution, panel management. Options: User Interviews (best for US market), Respondent (broader market), Prolific (academic quality, good for surveys), internal panel (cheapest, most controlled).

**The evaluation criteria.** For each tool: (1) Does it do the job well? (2) Does it integrate with our other tools? (3) Can the team learn it quickly? (4) What's the total cost (license + time + training)? (5) Will it scale with our research volume?


## The Research Practitioner's Operating System

### Mental Models for Research Thinking

**The Map-Territory Model.** All research produces maps, not territories. A persona is a map of the user, not the user. A market sizing is a map of the market, not the market. Every map simplifies, distorts, and omits. The skill is knowing what your map captures well and what it misses. Decisions made from a map that's treated as the territory are the most dangerous decisions in research.

**The Precision-Accuracy Tradeoff.** Precision is how specific your measurement is (the market is $4.275B). Accuracy is how close that measurement is to reality. Research can be precise and inaccurate (a detailed estimate based on wrong assumptions) or imprecise and accurate (a rough estimate that's directionally correct). For most business decisions, directional accuracy matters more than decimal precision.

**The Confirmation Bias Model.** Humans seek evidence that confirms what they already believe. Researchers are humans. The discipline: before starting research, write down what you expect to find. Then deliberately look for evidence that contradicts your expectation. If you only find confirming evidence, you probably have confirmation bias — redesign the study to test the opposite hypothesis.

**The Sample-Population Gap.** Every research finding is based on a sample. The question is always: does this sample represent the population you care about? 10 interviews with power users don't represent casual users. Always state the population your findings apply to and the populations they don't.

**The Diminishing Returns Model.** The first 5 interviews produce 80% of the insights. The next 5 produce 15%. Know when to stop. When the last 2-3 sessions produce no new themes, you've reached saturation.

### The 10 Rules of Research

1. **Start with the decision.** Every study must answer: what decision will this research inform? No decision = no research.
2. **Behavior > opinion.** What people DO is more reliable than what people SAY. Observe behavior whenever possible.
3. **Specificity beats generality.** "Users find checkout confusing" is useless. "3 of 5 users couldn't find shipping cost before clicking Place Order" is actionable.
4. **Triangulate methods.** No single method reveals the full truth. Combine qualitative (why) with quantitative (how many).
5. **Sample deliberately.** Who you study determines what you find. Choose participants who represent the population you're making decisions about.
6. **Acknowledge uncertainty.** All research has limitations. State them. Confidence without acknowledging uncertainty is arrogance, not evidence.
7. **Speed beats perfection.** Directionally correct research delivered in time beats perfect research delivered after the decision.
8. **Synthesis is the skill.** Data collection is mechanical. Synthesis — turning data into insight — is the craft.
9. **Communicate for action.** Present findings as: recommendation + evidence + trade-offs. Not 47 findings — the 3-5 that matter.
10. **Build institutional memory.** Every study should be findable and reusable. The repository is compound interest.

### The Research Career Progression

**Junior (0-2 years):** Master the methods. Conduct interviews, run usability tests, design surveys, analyze data. Focus on execution quality.

**Mid (2-5 years):** Master synthesis. Turn data into insights. Develop storytelling skills. Begin advising on research strategy. Own end-to-end studies.

**Senior (5-8 years):** Master influence. Ensure research changes decisions. Build stakeholder relationships. Mentor juniors. Connect research to business outcomes.

**Lead/Director (8+ years):** Master the system. Build research operations. Hire and develop the team. Represent research at the executive level. Shape company strategy through research.


## When to use

When anomaly detection is the right method for the research question at hand. When decision stakes are high enough to justify the investment. When existing data is insufficient and new evidence is needed. When the team is operating on assumptions that haven't been validated.
