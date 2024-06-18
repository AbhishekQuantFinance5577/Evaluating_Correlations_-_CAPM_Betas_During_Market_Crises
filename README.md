# Evaluating_Correlations_-_CAPM_Betas_During_Market_Crises
This project analyzes whether correlations between stocks and CAPM betas increase during market crises using daily returns data for S&amp;P 500 stocks from 1980 to 2023. The study identifies market crises and evaluates statistical patterns to confirm or refute the saying "correlations go to one" during these periods.


### Project Description: Evaluating Correlations and CAPM Betas During Market Crises

#### Purpose
This project aimed to achieve two goals:
1. Learn to calculate and evaluate return statistics for panel data in Python.
2. Evaluate the popular financial market saying that “correlations go to one” during crises and determine if a similar pattern exists for CAPM betas.

#### Assignment
The project focused on convincing whether correlations between stocks in the S&P 500 and CAPM betas increase during market crises.

#### Implementation Details
1. **Data Collection:**
   - Used daily returns for current stocks in the S&P 500 from 1980 to 2023.
   - Utilized `sp500.csv`, which includes daily closes for the S&P 500 (ticker ^GSPC) from 1927 to 2023.
   - Additional data was downloaded using the `pandas-datareader` and `yfinance` packages.

2. **Defining Crises:**
   - A crisis begins with a bear market (a 20% decline in the S&P 500 from its recent peak).
   - A crisis ends with the next bull market (a 20% rise in the S&P 500 from its recent trough).
   - Continuous measures of market performance, such as drawdowns and recent runups, were also considered.

3. **Analysis:**
   - Evaluated monthly and quarterly windows.
   - Calculated summary statistics (e.g., mean and median) for correlations and CAPM betas.
   - Used the following formulas:
     - **Correlation:** \(\rho_{i,j} = \frac{\text{Cov}(i,j)}{\text{Std}(i) \cdot \text{Std}(j)}\)
     - **CAPM Beta:** \(r_{i,t} = r_{f,t} + \beta_i (r_{m,t} - r_{f,t}) + \epsilon_{i,t}, \text{ where } \beta_i = \frac{\text{Cov}(i,m)}{\text{Var}(m)}\)

4. **Findings:**
   - Analyzed how correlations between stocks and CAPM betas changed during identified market crises.
   - Verified if correlations tended to increase ("go to one") during these periods.
   - Examined if CAPM betas exhibited similar patterns.

5. **Visualization and Reporting:**
   - Created clear plots and concise bulleted explanations to illustrate findings.
   - Highlighted any weaknesses in the analysis and proposed potential solutions.

#### Outcomes
- Confirmed that correlations between stocks in the S&P 500 increase during market crises, supporting the saying "correlations go to one."
- Identified similar patterns for CAPM betas, with notable increases during crises.
- Provided a comprehensive analysis with visual evidence to support findings, along with discussions on the limitations and robustness of the results.
