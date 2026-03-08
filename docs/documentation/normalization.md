# Normalization

Three normalization options are available in FragPipe-Analyst:

- **No normalization** (default): The input data are not further normalized, as they are assumed to have already been normalized by the FragPipe quantification tools (e.g., TMT-I median normalization for TMT data).
- **Variance-stabilizing normalization (VSN)**: Performed using the R package `vsn`. It simultaneously normalizes and stabilizes the variance across the intensity range. Available only for LFQ and DIA data.
- **Median centered**: The quantification values of each sample are shifted by subtracting the sample median, aligning the median intensity across all samples.
