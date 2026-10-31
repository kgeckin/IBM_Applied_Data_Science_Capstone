# Final Capstone Presentation

**SpaceX Falcon 9 First Stage Landing Prediction**

The presentation follows the original 47-slide IBM / Coursera capstone template. The design, original section sequence, cover and slide numbering have been retained. Presentation content is based on the project's notebooks, SQL output, saved datasets and data visualizations.

## Deliverables

| File | Format | Purpose |
| --- | --- | --- |
| [Completed presentation](IBM_SpaceX_Capstone_Original_Coursera_Template_Evidence_Added.pptx) | PPTX | Editable, 47-slide original-template deck |
| [Presentation export](IBM_SpaceX_Capstone_Original_Coursera_Template_Evidence_Added.pdf) | PDF | 47-page review and submission copy |

**Upload status:** The two binary deliverables are being staged for upload. Links above will work once both files have been uploaded to this folder. Review this pull request only after confirming both files are present.

## Presentation evidence

The deck includes:
* Short notebook code excerpts and linked source references for API collection, web scraping, data wrangling and exploratory analysis.
* SQL query excerpts with their recorded notebook results on the corresponding SQL slides.
* Charts for launch sites, orbit types, payloads and yearly landing trends.
* Reconstructed charts using the available saved geospatial and dashboard CSV datasets.
* Classifier accuracy comparison and a confusion matrix from the saved notebook outputs.

The small code panels are **presentation-ready excerpts**, not literal screenshots of every notebook cell. A code panel may abbreviate implementation details. The linked notebooks remain the authoritative code source.

## Source notebooks

| Topic | Source |
| --- | --- |
| SpaceX API | [Module 1 API notebook](../Module1/1-jupyter-labs-spacex-data-collection-api.ipynb) |
| Web scraping | [Module 1 scraping notebook](../Module1/2-jupyter-labs-webscraping.ipynb) |
| Data wrangling | [Module 1 wrangling notebook](../Module1/3-labs-jupyter-spacex-Data%20wrangling.ipynb) |
| SQL exploration | [Module 2 SQL notebook](../Module2/4-jupyter-labs-eda-sql-coursera_sqllite.ipynb) |
| Launch site maps | [Module 3 Folium notebook](../Module3/5-lab-jupyter-launch-site-location-v2.ipynb) |
| Interactive dashboard | [Module 3 Dash source](../Module3/spacex_dash_app.py) |
| Machine learning | [Module 4 prediction notebook](../Module4/6-SpaceX-Machine-Learning-Prediction-Part-5-v1.ipynb) |

## Results and caveats

All four classifiers reported approximately **83.3% test accuracy** on the notebook's **18-observation** held-out sample. The notebook's cross-validation scores differ by classifier. Decision Tree reported the highest saved mean cross-validation score (87.5%).

**Important evaluation caveat:** The saved modeling notebook applies StandardScaler to the full feature matrix before train/test splitting. This creates possible preprocessing leakage. A stronger follow-up analysis would fit preprocessing within the training folds using a Pipeline, then reevaluate the models. Treat the reported accuracy as an educational notebook result rather than an independent production benchmark.

The saved course materials include related but not perfectly identical datasets. Some map and dashboard images in the presentation were reconstructed from saved CSVs, rather than captured as live Folium or Dash screenshots.

## Before submitting to Coursera

1. Verify the PPTX and PDF each show 47 pages and match the original IBM template.
2. Open the PDF to check every code panel, chart, SQL result and hyperlink.
3. Confirm that source links open the correct notebook or source script.
4. Check any rubric requirements for an actual Folium map or Plotly Dash screenshot. Reconstructed plots may not fulfill those requirements.
5. Confirm that the final evaluation route and remaining assignments are complete in your own Coursera account.

## Source preservation

The original Coursera template was not overwritten. The PPTX and PDF listed above are separate output artifacts. This repository does not contain customer, employer or internal infrastructure information.
