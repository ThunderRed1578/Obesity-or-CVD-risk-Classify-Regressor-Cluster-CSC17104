<h1 style="text-align: center;"> 
    <span style="font-size: 40px; font-weight: bold">
        CSC17104 – PROGRAMING FOR DATA SCIENCE
    </span>
</h1>

<div style="text-align: center;"> 
    <span style="font-size: 32px; font-weight: bold">
        FINAL PROJECT
    </span>
</div>

<div style="text-align: center;"> 
    <span style="font-size: 24px; font-weight: bold">
        <i>
            Data Collecting
        </i>
    </span>
</div>

<div style="text-align: right;">
    <span style="font-size: 14px">
        <i>
            Nov 22, 2025
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

I. [Subject](#i)

1. [Subject](#i_1)

2. [Topic, Domain, and Phenomenon](#i_2)

3. [Real-World Context](#i_3)

II. [Source](#ii)

III. [Licensed](#iii)

IV. [Collection Methodology](#iv)

V. [Reason for choosing](#v)

1. [About the topic](#v_1)

2. [Potential Questions & Insights](#v_2)

---

<h1 id="i" style="font-weight: bold">I. Subject</h1>

<h2 id="i_1" style="font-weight: bold">1. Subject</h2>

The primary subject of this dataset is the Estimation of Obesity Levels based on individual lifestyle choices and demographic factors.

It focuses on determining how various eating habits and physical activities correlate with a person's weight category, ranging from "Underweight" to "Obesity Type III."

<h2 id="i_2" style="font-weight: bold">2. Topic, Domain, and Phenomenon</h2>

**Topic:** `Lifestyle` vs. `Health Outcomes`. The data explores the causal or correlational relationship between daily behaviors and physiological health. It specifically looks at:

* Dietary Intake: Frequency of high-calorie food, vegetables, water, and alcohol.

* Energy Expenditure: Physical activity levels and sedentary behavior (time spent on technology).

**Domain:** This dataset sits at the intersection of two major domains:

* Public Health & Nutrition: The study of epidemiology and metabolic health.

* Data Science (Classification): This is a labeled dataset designed for Machine Learning. It is structured for training algorithms to predict a categorical target variable (NObesity) based on feature inputs.

**Phenomenon:** The data describes the progression of Body Mass Index (BMI). It captures the phenomenon where specific combinations of environmental factors (transportation), behavioral factors (snacking, exercise), and biological factors (age, gender) result in specific weight classifications.

<h2 id="i_3" style="font-weight: bold">3. Real-World Context</h2>

This data represents a sociological and medical survey conducted in Latin America (specifically Mexico, Peru, and Colombia). It reflects several real-world contexts:

* **The Global Obesity Epidemic:** It addresses the growing public health concern regarding rising obesity rates, particularly in developing nations where dietary habits are shifting.

* **Sedentary Lifestyle Impact:** By including attributes like Time using technology devices (TUE) and Transportation used (MTRANS), the data represents the modern context where technology and urbanization contribute to lower physical activity.

* **Preventative Health Screening:** In a real-world scenario, this data represents the kind of information a nutritionist or health app might collect to assess a patient's risk profile without needing expensive medical testing—relying instead on self-reported habits.

---

<h1 id="ii" style="font-weight: bold">II. Source</h1>

**Platform:**  

* Kaggle

* URL: [Obesity or CVD risk (Classify/Regressor/Cluster)](https://www.kaggle.com/datasets/aravindpcoder/obesity-or-cvd-risk-classifyregressorcluster)

**Author:**

* Fabio Mendoza Palechor

* Alexis de la Hoz Manotas

**Publication date:** 2023

---

<h1 id="iii" style="font-weight: bold">III. Licensed</h1>

**Licensed:** [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)  

The Creative Commons Attribution-ShareAlike 4.0 International license (`CC BY-SA 4.0`) allows licensees to exercise the following freedoms:  

* Share - We are free to copy and redistribute the material in any medium or format for any purpose, even commercially.  

* Adapt - We are free to remix, transform, and build upon the material for any purpose, even commercially.  

Since the license explicitly permits commercial uses, educational use, which is typically non-commercial, is fully permitted under the terms.

**Attribution Requirements:**

* Give appropriate credit.

* Provide a link to the license.

* Indicate if changes were made.

* Must do this in any reasonable manner, but not in any way that suggests the licensor endorses we or our use.

* Should also retain a copyright notice and a notice about the disclaimer of warranties, and a URI if reasonable.

* If the licensor requests that we remove identifying credit (e.g., their name), we must comply with this request to the extent practical.

**Usage Restrictions and Obligations:**

* **ShareAlike Condition:** If we remix, transform, or build upon the material (create an adaptation), we must distribute our contributions under the same license as the original (CC BY-SA 4.0).

* **No Additional Restrictions:** We are prohibited from applying legal terms or effective technological measures (like Digital Rights Management or DRM) that legally restrict others from exercising the rights the license permits.

* **Termination:** The license terminates automatically if we fail to comply with its terms. If the material is under a 4.0 license, our rights are automatically reinstated if we fix the problem within 30 days of discovery.

* **No Warranty:** The license does not contain a warranty. We should note that the license may not give us all the permissions necessary for our intended use, as other rights (such as publicity, privacy, or moral rights held by third parties) may still limit how we use the material. If we are concerned about third-party rights, we may want to clear those rights in advance.

* **Public Domain Exceptions:** We do not have to comply with the license terms for elements of the material that are in the public domain or when our use is permitted by an applicable exception or limitation to copyright (such as fair use or fair dealing). These uses are unregulated by the license.

* **Non-binding Requests:** Licensors may indicate non-binding requests (such as asking licensees to mark or describe changes they make). While it is our option and not an obligation, it is recommended to comply with these requests when reasonable.

---

<h1 id="iv" style="font-weight: bold">IV. Collection Methodology</h1>

* The data was anonymously collected from web surveys

* The data collect from people from the countries of Mexico, Peru and Colombia, with ages between 14 and 61 and diverse eating habits and physical condition

---

<h1 id="v" style="font-weight: bold">V. Reason for choosing</h1>

<h2 id="v_1" style="font-weight: bold">1. About the topic</h2>

* **The "Modern Lifestyle" Paradox:** The dataset includes attributes like Time using technology devices (`TUE`) and Transportation used (`MTRANS`). This allows for an analysis of how modern conveniences (sedentary jobs, driving, screen time) are contributing to the obesity epidemic.

* **Granularity of Classification:** Unlike simple datasets that might just label someone as "Obese" or "Not Obese," this dataset offers 7 distinct levels (from `Underweight` to `Obesity III`). This allows for much more nuanced insights into the progression of weight gain.

* **Cultural Specificity:** Because the data comes from Mexico, Peru, and Colombia, it reflects dietary habits specific to Latin America. This is valuable for avoiding the "Western bias" often found in health datasets that focus only on the US or Europe.

* **Psychological/Behavioral Component:** Attributes like Calories consumption monitoring (`SCC`) touch on the psychological aspect of weight management - does simply tracking calories lead to better outcomes?

<h2 id="v_2" style="font-weight: bold">2. Potential Questions & Insights</h2>

<h3 id="v_2_a" style="font-weight: bold">a. Behavioral Correlations (Cause & Effect)</h3>

* **Technology vs. Health:** Is there a strong positive correlation between high Time using technology (`TUE`) and `Obesity Type III`?

* **The Impact of Transport:** Do individuals who use "Public Transportation" or "Walking" have significantly lower BMI than those who use Automobiles?

* **Snacking vs. Main Meals:** Which contributes more to obesity levels: the number of main meals (`NCP`) or the frequency of consumption of food between meals (`CAEC`)?

<h3 id="v_2_b" style="font-weight: bold">b. Dietary Analysis</h3>

* **The Alcohol Factor:** How does alcohol consumption (`CALC`) vary across the different obesity classes? Is it a significant differentiator?

* **Water Intake:** Does high daily water consumption (CH2O) act as a protective factor against higher levels of obesity?

* **Vegetable Frequency:** Is the frequency of vegetable consumption (FCVC) a strong enough predictor to distinguish between "Overweight" and "Normal" weight, or is it only effective at the extremes?

<h3 id="v_2_c" style="font-weight: bold">c. Predictive Modeling (Machine Learning)</h3>

* **Feature Importance:** If we build a Random Forest or Decision Tree model, which variable will be the "Root Node"? (i.e., What is the single most important factor in determining a person's obesity level - is it their genetics/family history, or their physical activity?)

* **Undiagnosed Classification:** Can we accurately classify a user's obesity level based only on their answers to the survey questions (habits), without actually measuring their weight or height? This would be useful for telemedicine apps.
