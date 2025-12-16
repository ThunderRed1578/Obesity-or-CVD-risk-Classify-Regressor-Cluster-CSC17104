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

<h2 id="iii_1" style="font-weight: bold">1. Question</h2>

<h2 id="iii_2" style="font-weight: bold">2. Meaningful & Challenging</h2>

<h2 id="iii_3" style="font-weight: bold">3. Motivation & Benefits</h2>

---

<h1 id="iv" style="font-weight: bold">IV. Question 4: (điền câu hỏi vào)</h1>

<h2 id="iv_1" style="font-weight: bold">1. Question</h2>

<h2 id="iv_2" style="font-weight: bold">2. Meaningful & Challenging</h2>

<h2 id="iv_3" style="font-weight: bold">3. Motivation & Benefits</h2>

---

<h1 id="v" style="font-weight: bold">V. Question 5: The Impact of Digital Lifestyle (TUE) and Physical Activity (FAF) on Obesity</h1>

<h2 id="v_1" style="font-weight: bold">1. Question</h2>

How does the correlation between time spent using technology devices (`TUE`) and physical activity frequency (`FAF`) impact obesity levels? Specifically, can maintaining a high frequency of physical activity (high `FAF`) effectively mitigate or neutralize the weight gain risks associated with a sedentary lifestyle caused by prolonged technology use (high `TUE`)?

<h2 id="v_2" style="font-weight: bold">2. Meaningful & Challenging</h2>

**Meaningful:**

* **Real-World Relevance:** This analysis addresses one of the most pressing public health issues of the modern era: The Sedentary Lifestyle. In a digital age where screen time (`TUE`) is unavoidable for work and study, understanding its direct correlation with health is critical.

* **Practical Value:** It moves beyond theoretical observation to provide a clear picture of how modern habits impact physical well-being.

**Challenging:**

* **Analytical Depth:** The relationship is not simply linear. This analysis requires examining the interaction between opposing forces: the passive nature of Technological Sedentarism versus the active nature of Physical Effort.

* **Complex Visualization:** It requires multi-dimensional visualization techniques to locate the "balance point," rather than a simple comparison of variable A to variable B.

<h2 id="v_3" style="font-weight: bold">3. Motivation & Benefits</h2>

**Why is this question worth investigating?**

* To decode the common myth: "Can diligent exercise completely offset the physiological harm of sitting at a computer all day, or is the damage irreversible?"

**What benefits or insights would answering this question provide?**

* **Decoding Myths:** It provides a definitive answer to whether exercise can neutralize the effects of prolonged screen time.

* **Practical Recommendations:** Instead of generic advice, it yields specific insights (e.g., "If you sit for >5 hours, you specifically need Activity Level > 2 to maintain weight").

* **Social Value:** The findings are directly applicable to high - risk demographics like office workers and students, offering them a scientific basis for lifestyle changes.

**Who would care about the answer?**

* **Target Audience:** Office workers, IT students/professionals, and anyone with a desk job - demographics at the highest risk of obesity.

**What real-world problem does this inform?**

* **Actionable Advice:** Instead of generic advice like "exercise more," this analysis provides specific, data-driven thresholds.

* **Example Outcome:** Determining if a user has a TUE > 5 hours, they specifically need a FAF > 2 to maintain weight, enabling precise lifestyle adjustments.

---

<h1 id="vi" style="font-weight: bold">VI. Question 6: Multivariate Analysis of Meal Frequency (NCP) and Water Consumption (CH2O)</h1>

<h2 id="vi_1" style="font-weight: bold">1. Meaningful & </h2>

How does the combination of the number of main meals (`NCP`) and daily water consumption (`CH2O`) contribute to the classification of obesity levels? Is there an optimal behavioral pattern (e.g., "Eating frequent small meals combined with high water intake") that maintains "Normal" weight and is statistically distinct from the behaviors of obesity groups?

<h2 id="vi_2" style="font-weight: bold">2. Meaningful & Challenging</h2>

**Meaningful:**

* **Scientific Validation:** There is an abundance of anecdotal advice (e.g., "eat small frequent meals," "drink water to lose weight"). This analysis is meaningful because it turns those rumors into statistical hypotheses, verifying truth versus fiction using real data.

* **Decision Making:** It provides a scientific basis for dietary planning rather than relying on intuition.

**Challenging:**

* **Technical Complexity:** This cannot be answered with raw data alone. It involves a multi-step workflow including Feature Engineering (creating "Healthy" vs. "Unhealthy" user groups).

* **Statistical Rigor:** It requires the use of statistical tests (such as T-tests) to prove that observed differences are statistically significant and not just random noise.

<h2 id="vi_3" style="font-weight: bold">3. Motivation & Benefits</h2>

**Why is this question worth investigating?**

* To uncover unexpected insights, such as determining if water intake is a stronger predictor of weight control than meal frequency, allowing for prioritized efforts.

**What benefits or insights would answering this question provide?**

* **Actionable Strategy:** Users will gain a specific blueprint for success (e.g., identifying that ">2L Water + 4 Meals/day" is the most effective combo), rather than guessing.

* **Prioritization of Efforts:** It uncovers which factor is more critical—hydration or meal frequency - allowing people to focus their limited energy on what matters most for weight loss.

**Who would care about the answer?**

* **Target Audience:** Individuals seeking weight loss, nutritionists, and health coaches looking for optimized strategies.

**What real-world problem does this inform?**

* **Actionable Strategy:** It aims to produce a clear "Action Formula."

* **Example Outcome:** Users will understand the specific combination (e.g., >2L Water + 4 Meals/day) that yields the best results, optimizing their weight loss journey by focusing on factors that actually move the needle.