
# Financial Portfolio Analysis and Optimization

### Project Description
This project focuses on the analysis and optimization of financial portfolios using momentum strategies and portfolio evaluation. Based on historical Nasdaq data and various financial parameters, it explores different approaches to building optimized portfolios and evaluates their performance over time.

### Project Structure
The project is divided into multiple notebooks, each covering a specific stage of the analysis:

1. **0_DataAcquisition.ipynb**: Data Acquisition
   - Downloads historical data for the NASDAQ 100, including price history and index composition over the last ten years (2014-2023).
   - Prepares the data by checking data quality and handling missing values.
   - Computes logarithmic returns for stocks and the reference index.

2. **1_Nasdaq_Compositions.ipynb**: Nasdaq Index Composition Reconstruction
   - Reconstructs the NASDAQ 100 composition over the years, tracking stocks that were added or removed.
   - Organizes the data to represent the full history of the index.

3. **2_logReturnsRegression.ipynb**: Rolling Regression of Logarithmic Returns
   - Imports the previously acquired data and calculates net returns using the Fama and French Three-Factor Model.
   - Executes a rolling regression on the logarithmic returns for each stock to compute necessary parameters.
   - Extracts p-values to analyze parameter significance.

4. **3_Portfolios_Evaluation.ipynb**: Portfolio Creation and Evaluation
   - Builds portfolios using various metrics like Sharpe ratio, systematic and specific risks, and expected returns.
   - Includes functions to visualize portfolio performance compared to the NASDAQ 100 benchmark.
   - Conducts an alpha analysis to identify stocks with significant parameters and creates balanced portfolios.

5. **4_Momentum_Strategy.ipynb**: Momentum Strategy
   - Calculates an HQM (High Quality Momentum) score for each stock, based on momentum indicators over various time windows (180, 90, 60, 30, and 7 days).
   - Creates portfolios based on top momentum stocks and compares their performance against the benchmark.
   - Includes evaluation metrics and visualizations to assess portfolio performance.

### Requirements and Dependencies
Ensure the following libraries are installed:
- `pandas`
- `numpy`
- `matplotlib`
- `scipy`
- `sklearn`

### Installation Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/Corsi01/InvestmentPortfolio-Optimization.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   *(I can help generate a `requirements.txt` file if needed)*

### Usage Examples
Each notebook can be executed sequentially. It is recommended to start with **0_DataAcquisition.ipynb** to ensure all necessary data is acquired and prepared for subsequent analyses.

### Results
The project provides a detailed evaluation of portfolio performance using metrics such as Sharpe ratio, specific and systematic risks, and expected returns. Graphs are included to compare portfolio performance against the NASDAQ 100 benchmark.

### Contributors
- **Corsi01**
- *(List any collaborators here)*

### License
This project is licensed under the MIT License. 
