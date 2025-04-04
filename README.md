# time-series-analysis-using-R-shiny
📈 A Shiny dashboard for interactive time series analysis. Supports CSV/Excel upload, plotting, decomposition, stationarity tests, SARIMA, GARCH, smoothing methods, and PDF report export. Ideal for researchers, analysts, and students.
This Shiny dashboard application provides an interactive platform for performing comprehensive time series analysis. Users can upload time series data in either CSV or Excel format and select the variable of interest for analysis. A user-defined frequency input allows flexibility for different types of time series, such as monthly, quarterly, or annual data.

Upon triggering the analysis, the app generates a time series plot and a decomposition graph that breaks down the series into trend, seasonal, and residual components. It also conducts a stationarity check using the Augmented Dickey-Fuller (ADF) test and provides an interpretation of whether the data is stationary.

For advanced analysis, users can select from a range of optional tools. These include Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) plots to help identify model structures. The app can automatically fit a Seasonal ARIMA (SARIMA) model using auto.arima(), with detailed outputs including residual diagnostics, the Ljung-Box test for independence, and the Shapiro-Wilk test for normality of residuals.

Smoothing techniques are also available: users can apply a simple moving average, exponential smoothing, or Holt-Winters smoothing to smooth the time series and highlight trends. For modeling volatility in time series data, a GARCH(1,1) model can be fitted using the rugarch package, with outputs including a summary, volatility plot, and model diagnostics.

A notable feature of the application is its ability to generate a downloadable PDF report summarizing all selected analyses. This report is created using R Markdown and includes plots, statistical tests, and model summaries, making it suitable for research, presentations, or business reporting.

The app is built using R and leverages key packages such as shiny, shinydashboard, ggplot2, forecast, tseries, TTR, rugarch, and rmarkdown. It is ideal for analysts, researchers, students, and professionals seeking a flexible and efficient tool for time series data exploration and modeling.
