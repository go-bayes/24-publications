
We can illustrate this with a simple numerical example.

Suppose a population of  200 individuals divided into two age cohorts: **Younger Cohort:** 100 individuals;**Older Cohort:** 100 individuals. Suppose in the **Younger Cohort** there is a 30% chance of receiving treatment, thus Treated: 30 individuals Untreated: 70 individuals. Suppose further in the **Older Cohort:** there is a 70% chance of receiving treatment. Treated: 70 individuals; Untreated: 30 individuals. Furhther suppose the treatment increases happiness by **10 points** on a standardised scale, and baseline happiness for all individuals is **50 points**.

Now, let's calculate the average happiness scores for each cohort.

1. **Younger Cohort:**

   - **Treated Individuals:**
     - Happiness Score: $50 \, (\text{baseline}) + 10 \, (\text{treatment effect}) = 60$
     - Total Happiness: $30 \, (\text{individuals}) \times 60 = 1,800$
   - **Untreated Individuals:**
     - Happiness Score: $50 \, (\text{baseline})$
     - Total Happiness: $70 \, (\text{individuals}) \times 50 = 3,500$
   - **Average Happiness:**
     - $\frac{1,800 + 3,500}{100} = \frac{5,300}{100} = 53$

2. **Older Cohort:**

   - **Treated Individuals:**
     - Happiness Score: $50 + 10 = 60$
     - Total Happiness: $70 \times 60 = 4,200$
   - **Untreated Individuals:**
     - Happiness Score: $50$
     - Total Happiness: $30 \times 50 = 1,500$
   - **Average Happiness:**
     - $\frac{4,200 + 1,500}{100} = \frac{5,700}{100} = 57$

Our finding is that: **Younger Cohort Average Happiness:** = 53, and **Older Cohort Average Happiness:** 57
Even though the treatment effect is constant (10 points) for both cohorts, the **older cohort shows a higher average happiness score**. This arises from the higher proportion of treated individuals in the older cohort (70%) compared to the younger cohort (30%). The increased average treatment effect in the older cohort arises from the conditional randomisation based on age, not from a difference in the treatment's efficacy.

This example demonstrates that when randomisation occurs conditional on a measurable feature such as age, and the treatment effect is constant, differences in treatment probabilities across groups can lead to variations in observed average treatment effects. However, if adjust for this difference in the probability of receiving treatment, or simply compare treatment effects with the different age strata, the illusion of a different treatment group disappears. 