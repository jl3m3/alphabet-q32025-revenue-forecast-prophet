# alphabet-q32025-revenue-forecast-prophet
Project to forecast Alphabet(2025–2028) revenue, includes Segment Analysis (Cloud vs. Ads) and Bear/Base/Bull scenarios. Using Python and Meta's Prophet model. 

Why I chose Metas Prophet? 

1. **Interested** : This whole project started slowly and get bigger and bigger. Took more time than anticipated. Prophet should be quite good model to predict future revenues for SaaS companies.
2.  **Seasonality** : Alphabet has a massive Q4 holiday spike every year. Linear models treat this as noise. Prophet should decomposes the data using a **Fourier Series** to wrap around these spikes , ensuring it shouldn't mistake a Q1 drop for a business failure.
4. **Sympathetic Movement (Regressors):** Adding Amazon as a ´regressor´ into the model, a Pearson Correlation Coefficient of **0.99** between Alphabet and Amazon. 
5. **Changepoint Detection:** Prophet should automatically detect changes (like the 2023 AI boom and COVID) and adjusts the trend trajectory without manual intervention.
  
  
### The "Cloud Pivot" Hypothesis ### 
**The Thesis** Historically, Alphabet has been an advertising monopoly. Hypothesis is that **Google Cloud is "growing fast"** to become the primary driver of marginal revenue growth.

**The Data** Specific compounding growth rates ("Grades") for each business segment (this is based on the analyst reports and then taking more concervative approach): 

* **Ads (The Cash Cow):** Decaying growth (8% → 5%).
* **Cloud (The Engine):** Sustained high growth (28% → 20%).
* **Other (The Wildcard):** Moderate acceleration (17% → 19%).

### **Strategic Conclusion** 
The model confirms that while Ads will provide the bulk of the cash, 
**Google Cloud will generate the majority of new growth dollars** by 2028. 
This diversification reduces exposure to cyclical ad-spending downturns.

