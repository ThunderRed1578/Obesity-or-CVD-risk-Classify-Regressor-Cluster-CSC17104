<h1 style="text-align: center;"> 
    <span style="font-size: 40px; font-weight: bold">
        CSC17104 – PROGRAMING FOR DATA SCIENCE
    </span>
</h1>

<h2 style="text-align: center;"> 
    <span style="font-size: 32px; font-weight: bold">
        FINAL PROJECT
    </span>
</h2>

<h3 style="text-align: center;"> 
    <span style="font-size: 24px; font-weight: bold">
        <i>
            Asking Question
        </i>
    </span>
</h3>

<div style="text-align: right;">
    <span style="font-size: 14px">
        <i>
            Dec 8, 2025
        </i>
    </span>
</div>

> | Name | ID |
> | --- | --- |
> | Lê Võ Nhật Minh | 22120210 |
> | Nguyễn Hữu Nghĩa | 22120227 |
> | Nguyễn Lê Tấn Phát | 22120262 |

---

<h1 align="center">
    <span style="font-size: 40px; font-weight: bold">
        Mục lục
    </span style>
</h1>

I. [Question 1:](#i)

1. [Reason](#i_1)

2. [Benefit](#i_2)

3. [Necessary step](#i_3)

II. [Question 2:](#ii)

1. [Reason](#ii_1)

2. [Benefit](#ii_2)

3. [Necessary step](#ii_3)

III. [Question 3:](#iii)

1. [Reason](#iii_1)

2. [Benefit](#iii_2)

3. [Necessary step](#iii_3)

IV. [Question 4:](#iv)

1. [Reason](#iv_1)

2. [Benefit](#iv_2)

3. [Necessary step](#iv_3)

V. [Question 5:](#v)

1. [Reason](#v_1)

2. [Benefit](#v_2)

3. [Necessary step](#v_3)

VI. [Question 6:](#vi)

1. [Reason](#vi_1)

2. [Benefit](#vi_2)

3. [Necessary step](#vi_3)
---

<h1 id="i" style="font-weight: bold">I. Question 1: Does the habit of Calorie Consumption Monitoring (SCC) significantly mitigate or reverse the risk of severe obesity among individuals who otherwise maintain unhealthy dietary patterns, specifically High Caloric Food Intake (FAVC) or Alcohol Consumption (CALC)?</h1>

<h2 id="i_1" style="font-weight: bold">1. Reason</h2>

* **New Weight-losing Hypothesis (Meaningful)**: Many people struggle to change what they eat. If data shows that simply tracking what they eat (even if it's high-calorie) reduces obesity, it suggests a more accessible entry point for weight management than strict dieting.

* **Technical Complexity (Challenging)**: This inquiry is analytically challenging because it transcends simple correlation to investigate conditional interaction effects requiring a multi-step workflow to isolate specific high-risk cohorts (high `FAVC`/`CALC`) and rigorously handle the severe class imbalance of the `SCC` feature. It cannot be solved with basic aggregation; instead, it demands statistical hypothesis testing (e.g., Chi-square or T-tests) and comparative visualization to distinguish true behavioral impact from random noise, thereby demonstrating deep critical thinking about the efficacy of self-monitoring interventions.

<h2 id="i_2" style="font-weight: bold">2. Benefit</h2>

* **Validation of Self-Monitoring Tools**: If `SCC` is proven effective even with a bad diet, it provides strong validation for the efficacy of health apps and fitness trackers (like MyFitnessPal) as a primary intervention tool.
* **Targeted Intervention Strategies**: If the answer is "No" (monitoring doesn't help if you eat junk), then health programs must stop focusing on "counting calories" and shift entirely to "quality of food" for this specific demographic.
* **Health App Developers**: Companies developing diet-tracking applications need to know if their core feature (logging food) is effective for users who haven't yet improved their diet quality.
* **Dietitians and Nutritionists**: Professionals deciding whether to advise a client to "start tracking" or "change the menu" first.

<h2 id="i_3" style="font-weight: bold">3. Necessary step</h2>

* Filter the dataset to isolate a sub-population of 'high-risk' individuals—defined as those having `FAVC` = 'yes' OR `CALC` $\in$ {'Frequently', 'Always'}. 
* Within this specific group, we will perform a comparative analysis of the `NObeyesdad` (Obesity Level) distribution between those who monitor their calories (`SCC` = 'yes') and those who do not (`SCC` = 'no')
* Determine if there is a statistically significant difference in obesity rates.
---

<h1 id="ii" style="font-weight: bold">II. Question 2: Can we develop a multi-class classification Machine Learning model (e.g., Random Forest or XGBoost) to accurately predict individual Obesity Levels (NObeyesdad) and subsequently utilize SHAP (SHapley Additive exPlanations) values to prescribe a personalized, optimal roadmap of modifiable lifestyle changes (specifically FCVC, CH2O, TUE, FAF) that maximizes the probability of transitioning a subject from an 'Obese' category to a 'Normal' or 'Overweight' category?</h1>

<h2 id="ii_1" style="font-weight: bold">1. Reason</h2>

* **Personalization (Meaningful)**: Weight loss is not "one size fits all." Some people might need more water (`CH2O`), while others need less screen time (`TUE`). This approach respects individual biological and behavioral differences.
* **End-to-End Machine Learning Pipeline (Challenging)**: from data preprocessing (encoding, scaling) and model selection (handling multi-class targets) to complex Model Interpretability. It goes beyond prediction accuracy to perform Counterfactual Analysis (What-If scenarios), requiring sophisticated simulation to determine the 'optimal path' for feature manipulation, demonstrating advanced capability in both algorithm implementation and domain-specific problem solving.

<h2 id="ii_2" style="font-weight: bold">2. Benefit</h2>

* **Actionable "Prescriptions"**: instead of generic advice like "exercise more," the output is specific: "For you, reducing screen time is 2x more effective than eating more vegetables."
* **Resource Optimization**: Helps users focus their limited willpower on the habits that matter most for their specific body type.
* **Healthcare Providers**: Doctors can use this to generate data-backed lifestyle plans for patients.
* **End Users**: Individuals struggling with obesity who want an efficient path to weight loss.
* **Decision Support**: It informs the daily lifestyle choices of individuals. It solves the problem of "Analysis Paralysis" where people don't know where to start their weight loss journey.

<h2 id="ii_3" style="font-weight: bold">3. Necessary step</h2>

* Remove `BMI` column then train a supervised learning model using the full remained dataset to predict the `NObeyesdad` target. 
* Post-training, we will apply model interpretability techniques (SHAP/LIME) to individual instances classified as 'Obesity_Type_II' or 'III'. 
* By simulating changes in actionable features (e.g., increasing `FAF` by 1 unit, decreasing `TUE` to 0), we will quantify which specific behavioral modification yields the highest reduction in obesity probability for that specific user.
---

<h1 id="iii" style="font-weight: bold">III. Question 3: (điền câu hỏi vào)</h1>

<h2 id="iii_1" style="font-weight: bold">1. Reason</h2>

<h2 id="iii_2" style="font-weight: bold">2. Benefit</h2>

<h2 id="iii_3" style="font-weight: bold">3. Necessary step</h2>

---

<h1 id="iv" style="font-weight: bold">IV. Question 4: (điền câu hỏi vào)</h1>

<h2 id="iv_1" style="font-weight: bold">1. Reason</h2>

<h2 id="iv_2" style="font-weight: bold">2. Benefit</h2>

<h2 id="iv_3" style="font-weight: bold">3. Necessary step</h2>

---

<h1 id="v" style="font-weight: bold">V. Question 5: The Impact of Digital Lifestyle (TUE) and Physical Activity (FAF) on Obesity</h1>

<h2 id="v_1" style="font-weight: bold">1. Reason</h2>

* **High Relevance (Meaningful):** We live in a digital era where screen time (`TUE`) is unavoidable. This question addresses the most "pressing" issue of modern public health: The Sedentary Lifestyle.

* **Analytical Complexity (Challenging):** This relationship is not simply linear. We aren't just comparing A to B; we are examining the interaction between two opposing forces: Technological Sedentarism vs. Physical Effort. It requires multi-dimensional visualization techniques to find the balance point.

<h2 id="v_2" style="font-weight: bold">2. Benefit</h2>

* **Decoding Myths:** It answers a tough question, "Can diligent exercise completely offset the harm of sitting at a computer all day, or is the damage irreversible?"

* **Practical Recommendations:** Instead of generic advice like "exercise more," you can provide specific figures (e.g., If you use a computer for >5 hours, you need an activity level of `FAF` > 2 to maintain weight).

* **Social Value:** The analysis results are immediately applicable to office workers and IT students-the demographic groups at highest risk.

<h2 id="v_3" style="font-weight: bold">3. Necessary step</h2>

---

<h1 id="vi" style="font-weight: bold">VI. Question 6: Multivariate Analysis of Meal Frequency (NCP) and Water Consumption (CH2O)</h1>

<h2 id="vi_1" style="font-weight: bold">1. Reason</h2>

* **Scientific Verification (Meaningful):** There is a lot of anecdotal advice like "eat small frequent meals" or "drink lots of water to lose weight." This question turns those rumors into statistical hypotheses to verify whether they are true or false based on real data.

* **High Technical Requirement (Challenging):** To answer this, we cannot use raw data. We must perform Feature Engineering (creating user groups: "Healthy Group" vs. "Unhealthy Group") and use statistical tests (like T-tests) to prove that the difference is statistically significant, not random.

<h2 id="vi_2" style="font-weight: bold">2. Benefit</h2>

* **Actionable Strategy:** It provides a clear "action formula." Users will know exactly which specific combination (e.g., >2L water + 4 meals/day) yields the best results, rather than just trying to starve themselves.

* **Uncovering Unexpected Insights:** We might discover that drinking water is more critical than the number of meals, or vice versa. This helps optimize weight loss efforts by focusing on the most important factor.

<h2 id="vi_3" style="font-weight: bold">3. Necessary step</h2>