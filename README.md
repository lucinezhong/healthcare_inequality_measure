<h1>Examining Inequality in Healthcare Utilization During Pandemic Disruptions in the United States</h1>


<h2>Abstract</h2>
<p>
  Health crises like the recent COVID-19 pandemic have continuously disrupted healthcare utilization, particularly among non-COVID-19 patients.
  However, it remains unclear whether these disruptions are experienced equally across populations or disproportionately impact specific
  sociodemographic groups, and how these inequalities evolve over the course of the disruption.
</p>
<p>
  In this study, we analyze electronic health records from millions of patients across the United States during the COVID-19 pandemic and show
  that, compared with the pre-pandemic period (2019), there was an around <strong>45% decline</strong> in the number of patient visits during the
  pandemic period (2020–2022). By employing the <strong>Gini coefficient</strong> to measure disparities in healthcare utilization declines across
  different sociodemographic groups, we identify a consistent increase in health inequalities during the pandemic, most pronounced across
  <strong>age</strong> and <strong>income</strong> groups.
</p>
<p>
  The decline in <strong>telehealth usage</strong>, which served as an alternative to in-person visits, after April 2021, was found to be associated
  with rising healthcare inequalities. These findings underscore that sustaining adaptive healthcare delivery strategies, such as telehealth, may
  help mitigate systemic inequities during long-term public health emergencies.
</p>

<hr/>

<h2>Data</h2>
<li>State-level Gini coefficients by age group</li>
<li>State-level Gini coefficients by race and ethnicity</li>
<li>State-level Gini coefficients by education level</li>
<li>State-level Gini coefficients by income group</li>
<li>State-level Telehealth Usage</li>

<h2>Methdologies</h2>
<ul>
  <li>
    
    <strong>Gini Coefficient</strong>:
    Measures overall inequality in healthcare utilization across demographic groups within a given month.
    Values range from 0 (perfect equality) to 1 (maximum inequality); higher values indicate greater disparity.
    <p>
  <code>
    G(t) = 1 − ∑<sub>i=1</sub><sup>n</sup>
    [Y<sub>i</sub>(t) + Y<sub>i−1</sub>(t)]
    [X<sub>i</sub>(t) − X<sub>i−1</sub>(t)]
  </code>
</p>

<p>
  where <code>X<sub>i</sub>(t)</code> represents the cumulative proportion of the population at time <em>t</em>
  after including group <em>i</em>, and <code>Y<sub>i</sub>(t)</code> represents the cumulative proportion of patient
  visits in the electronic medical record (EMR) dataset at time <em>t</em> after including group <em>i</em>.
  Groups are ordered in ascending order of their share of patient visits to ensure proper construction of the
  Lorenz curve. Here, <code>n</code> denotes the total number of demographic groups.
  </li>

  <li>
    <strong>Index of Disparity (ID)</strong>:
    Captures the average absolute deviation of group-specific utilization rates from the overall population rate,
    normalized by the overall rate:
    <br/>
    <code>Index of Disparity = (∑ |R<sub>i</sub> − R<sub>overall</sub>|) / R<sub>overall</sub></code>
  </li>

  <li>
    <strong>Population-Weighted Index of Disparity (PWID)</strong>:
    Extends the Index of Disparity by weighting each group’s deviation by its population size:
    <br/>
    <code>PWID = (∑ |R<sub>i</sub> − R<sub>overall</sub>| · P<sub>i</sub>) / (R<sub>overall</sub> · P<sub>overall</sub>)</code>
  </li>

  <li>
    <strong>Population Attributable Proportion (PAP)</strong>:
    Estimates the proportion of overall utilization loss attributable to inequality by comparing the lowest-utilizing
    group to the overall population:
    <br/>
    <code>PAP = 1 − (R<sub>lowest</sub> / R<sub>overall</sub>)</code>
  </li>
</ul>

