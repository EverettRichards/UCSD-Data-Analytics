In this directory, you will find my Jupyter Notebook in .ipynb and .pdf form, as well as the actual dataset used (financials.csv).

For a concise viewing of the project, I recommend opening the PDF file.

In this project, I used data from all S&P500 stocks in 2018 to make investment recommendations to a user. These recommendations are based on a weighted cosine similarity between each given stock, and the user's portfolio as a whole. This means that the system recommends stocks that are *most similar* to the user's portfolio as a whole (weighted by the relative share of assets invested in that particular stock), while also noting the *least similar* stocks in order to encourage diversity in investment.

I have attached two images showcasing the results of this project. The first image, RecommendationSummary.png, shows a list of stocks the system did/did not recommend based on the arbitrary portfolio I provided. It also shows how similar the stocks are to the user's portfolio, using a number between 0 (least similar) and 1 (most similar).

The second image, DistributionOfStockSimilarities.png, shows a modified histogram of the similarity each S&P500 stock has to the user's portfolio. This histogram shows that a typical stock has a similarity score of approximately 0.47 when compared with the given portfolio, with few stocks being extremely similar or dissimilar.

This project involves basic Python data processing and visualization techniques using libraries such as NumPy, pandas, and MatPlotLib.
I also used my own custom cosine similarity function that weights the squares of traditional cosine similarity metrics to compute an average similarity to a multi-stock portfolio.
