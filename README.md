1.1  EXECUTIVE SUMMARY

Predictability remains one of the top challenges in Agile software delivery. Despite Agile’s popular
ity, teams often cannot answer the deceptively simple question: when will the backlog be finished? 
Methods such as Scrum and Kanban promise adaptability and customer value, but delivery slippage 
persists. Industry surveys and studies continue to rank forecasting as a critical weakness, reflecting 
Agile’s reliance on deterministic tools—velocity averages, burn-down charts, and cumulative flow 
diagrams—that project a single completion date while ignoring uncertainty.

Agile’s strength is its responsiveness to change, yet this very flexibility complicates prediction. Iter
ative delivery, emergent requirements, and varying sprint velocities make forecasting inherently prob
abilistic, not deterministic. Nevertheless, most Agile practices treat schedule planning as a matter of 
extrapolating past velocity into the future. This creates a persistent mismatch between Agile’s dy
namic reality, and the static tools used to communicate progress. Stakeholders are often frustrated not 
by change itself, but by the lack of reliable foresight.

This dissertation investigates whether Monte Carlo simulation, a probabilistic method widely used in 
infrastructure and engineering projects, can be adapted to Agile contexts to model schedule risk. Un
like deterministic methods, Monte Carlo generates full distributions of outcomes, offering confi
dence-based ranges (e.g., P50 or P80) rather than a single forecast. While established elsewhere, such 
approaches remain rare in Agile software development, creating a gap between practice and potential.

1.1.1  AIM, OBJECTIVES, AND RESEARCH QUESTIONS 

The aim of this research is to evaluate whether Monte Carlo simulation can feasibly model schedule 
risk in Agile projects and what insights such an approach can provide.

The study pursued four objectives: 

• Develop a Monte Carlo artefact that translates Agile backlogs and sprint dynamics into prob
abilistic forecasts. 
• Identify and rank the main sources of schedule uncertainty.

• Derive actionable guidance from probabilistic outputs for Agile managers.

• Critically evaluate the model’s assumptions and scope.

These objectives were addressed through four guiding research questions (RQs):

• RQ1: How can Monte Carlo simulation be applied to model and quantify schedule risk in an 
Agile software project?

• RQ2: What are the key uncertainty factors in Agile project schedules, and how do they impact 
the probability of on-time delivery?

• RQ3: How can the results of a probabilistic schedule risk analysis inform decision-making 
and risk management in Agile projects?

• RQ4: What are the inherent limitations of the proposed simulation model, and to what extent 
are its findings generally agreed to other Agile contexts?

1.1.2  METHODOLOGY 

The research adopted a design science approach, constructing and testing a simulation artefact rather 
than only theorizing. A synthetic Agile backlog was modelled, with stochastic inputs for sprint ve
locity, scope churn, unplanned work, and discrete risks. The model was executed through 100,000 
Monte Carlo iterations. This ensured robust percentile forecasts while reducing statistical noise. 
Outputs were presented using standard statistical plots and evaluated across base, best, and worst
case scenarios. Sensitivity analysis was used to isolate the influence of individual variables, providing 
not just forecasts but explanatory insight into why schedules slipped. This approach allowed demon
stration of feasibility and exploration of uncertainty drivers while maintaining transparency and re
producibility.

1.1.3  KEY FINDINGS 

The research produced four main findings:

• Feasibility confirmed (RQ1). Monte Carlo simulation can be successfully applied in Agile 
contexts, producing distributions of completion outcomes that reveal both most-likely scenar
ios and the probability of overruns.

• Risk drivers identified (RQ2). Sensitivity analysis showed that:

o Velocity variance is the strongest predictor of schedule risk.

o Unplanned work is the second most influential factor, with backlog growth closely 
linked to slippage.

o Scope churn has a moderate effect.

o Discrete risks were least influential, though still present. These ranking challenges the 
literature’s focus on scope creep, highlighting velocity and unplanned work as under
explored drivers.

• Managerial guidance derived (RQ3). Probabilistic outputs support concrete recommenda
tions:

o Communicate forecasts as ranges (e.g., “80% chance of finishing by Sprint 3”), not 
fixed dates. 

o Add a one-sprint buffer to increase delivery confidence. 

o Maintain backlog discipline to minimise unplanned work. 

o Monitor and stabilise velocity variance, the single strongest risk indicator. 

• Limitations observed (RQ4). The model’s scope was constrained by:

o Use of synthetic rather than live project data.

o Fixed sprint cadence and independence assumptions.

o Limited validation against real-world outcomes. 

o Accessibility challenges for non-technical teams.

1.1.4  CONTRIBUTIONS 

The dissertation makes three main contributions:

• Theoretical: It reframes Agile risk by showing empirically that velocity variance and un
planned work, rather than scope creep, are the dominant drivers of uncertainty. This provides 
a corrective to existing literature, which has often privileged scope creep as the defining risk 
factor. The study therefore deepens the academic understanding of Agile uncertainty and 
aligns Agile scholarship more closely with observed delivery dynamics.

• Practical: It provides heuristics that Agile teams can use immediately: communicate probabil
istic ranges, add a one-sprint buffer, enforce backlog discipline, and track velocity stability. 
These recommendations are not abstract but directly implementable, equipping Product Own
ers and Scrum Masters with defensible practices to improve predictability and stakeholder 
communication.

• Methodological: It develops a reusable, transparent simulation artefact implemented in Python 
and Excel, demonstrating how design science can link academic concepts to practitioner tools. 
The artefact serves as a platform for future research, while also being applicable enough to 
adapt to real-world Agile project settings.

1.1.5  LIMITATIONS AND FUTURE RESEARCH 

The study’s reliance on synthetic data limits external validity. Future research should calibrate and 
validate the artefact against real Agile project datasets to test alignment between probabilistic fore
casts and actual outcomes. Extensions could also model interdependencies between risk factors, scale 
the artefact for multi-team contexts, and design practitioner-friendly dashboards. Such extensions 
would enhance both the robustness and the usability of probabilistic scheduling in Agile contexts. 

1.1.6  OVERALL SIGNIFICANCE 

This dissertation demonstrates that Monte Carlo simulation offers a feasible and valuable complement 
to Agile forecasting. It confirms that probabilistic methods can bridge Agile’s adaptability with quan
titative risk management, producing insights unavailable from deterministic tools. For academics, it 
advances Agile scholarship by reframing risk drivers and contributing a transparent artefact. For prac
titioners, it provides concrete heuristics that improve predictability, stakeholder communication, and 
delivery confidence. 

Ultimately, Monte Carlo simulation represents a methodological bridge—embedding rigorous risk 
analysis into Agile practice—thereby contributing to both the academic development of Agile meth
ods scholarship and the practical advancement of project delivery predictability. 
