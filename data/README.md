# Data

Raw review files are not committed. Google Play reviews include reviewer display names and profile-image URLs, so only aggregate results are published in `results/`.

To regenerate the data, run the notebooks in `notebooks/01_collect/`. Each one writes a CSV (for example `CelcomDiGI_reviews.csv`) with these fields:

`reviewId, userName, userImage, content, score, thumbsUpCount, reviewCreatedVersion, at, replyContent, repliedAt, appVersion`

Place the CSVs in the same folder as the analysis notebooks (or update `file_path` in each notebook) before running `notebooks/02_analyze/`.
