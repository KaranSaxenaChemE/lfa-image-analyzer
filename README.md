# LFA Image Analyzer

**A one-stop solution for automated LFA image and data analysis.**

For LFA researchers, developed by [Karan Saxena](https://www.karansaxena.in/)
and [Bhushan Toley](https://www.linkedin.com/in/bhushantoley/),
[Toley Lab](https://toleylab.weebly.com/), [Indian Institute of Science](https://iisc.ac.in/).

**[Open the app](https://karansaxenacheme.github.io/lfa-image-analyzer/)**

One workflow—from LFA images to quantitative results.

Tired of juggling image-analysis tools such as ImageJ, spreadsheets such as Excel, and coding tools (MATLAB, Python or R) for your LFA image and data analysis? This app brings those steps together in one unified workflow. Upload your images, choose your settings and run the analysis to get Test and Control measurements—or, for batch experiments, replicate statistics, calibration curves and calculated LoD. Your experimental images and analysis data stay on your own computer.

## Single LFA analysis

**Upload one strip image. Get its Test and Control line signals and T/C ratio.**

- **Automatic signal extraction:** detect Test and Control peaks without manually drawing separate measurement regions for each line.
- **Flexible quantification:** measure baseline-corrected integrated peak areas and peak prominences, with Test/Control ratios.
- **Multiple readouts:** analyse colorimetric, fluorescent or chemiluminescent strips containing one Test and one Control line.
- **Channel selection:** use automatic RGB selection or choose Red, Green, Blue, Grayscale or Contrast-Adjusted Grayscale.
- **Crop and inspect:** select the strip region and review channel profiles, shaded peaks and the profile aligned with the image.
- **Visible checks:** review input errors, detection warnings and measured values before using the results.
- **Save your results:** export measurement tables, editable SVG figures and an analysis PDF or self-contained HTML file with experimental notes.

## Batch LFA analysis

**Upload cropped strip images from your experiment. Get the calibration curve and calculated limit of detection (LoD)—all in one workflow.**

- **From images to calculated LoD:** select your image folder and analysis settings, then run image analysis, replicate statistics, calibration and LoD calculation without manually transferring intermediate measurements.
- **Organised experimental inputs:** concentration and replicate information are read from filenames. Include blank and concentration-series replicates for calibration and LoD calculation.
- **Sandwich and competitive assays:** use automatic format detection or select the format manually, with checks against the observed Test-line response.
- **Multiple readouts and channels:** process colorimetric, fluorescent or chemiluminescent strips containing one Test and one Control line, with automatic or manual channel selection.
- **Four signal choices:** Test peak area, Test/Control area ratio, Test peak prominence or Test/Control prominence ratio.
- **Six calibration models:** four-parameter logistic, five-parameter logistic, Hill, Langmuir, linear and two-term exponential.
- **Two LoD calculation methods:** choose between direction-aware, blank-based methods for sandwich and competitive responses.
- **Inspect the analysis:** review individual-strip diagnostics, replicate statistics, model equations, fitted coefficients, goodness-of-fit statistics and warnings.
- **Refit and export:** change the signal metric or calibration model without reprocessing images; export complete CSV tables, editable SVG figures, publication-formatted calibration plots and a notebook PDF or self-contained HTML file.

## Inputs and interfaces

Use 8-bit RGB images in JPG, JPEG, PNG, TIF or TIFF format. Orient each strip with
Control above Test. For Batch calibration, use filenames containing
`Concentration_ReplicateNumber_SubstrateName`, for example `0.1_II_AuNP.png`.
Replicates use uppercase Roman numerals. The included example strip is synthetic.

Single and Batch analysis open in the Notebook Interface; a separate Single App
Interface is also available. Review diagnostic figures, input checks and warnings
before using the results. Add experimental notes before saving the PDF or HTML file.

Both notebooks have **Save analysis as HTML** beside each PDF button. The saved
HTML embeds images, vector plots, complete tables, settings, experimental notes
and full analysis data in an interactive offline notebook. The saved file keeps
the left-side section menu, figure SVG and table CSV downloads, PDF saving and
editable experimental notes. Choose **Save updated HTML** to keep note edits in
a new file. Analysis settings and results stay locked; new calculations require
the app. No connection is needed to view or use the saved notebook's controls.
Files can be large when many images and figures are included.

## Use and citation

This app is free to use for analysis. A source-code reuse licence has not yet been
granted; licensing terms are under review. Third-party components retain their
respective licences.

If you use this app for image processing or data analysis of your lateral flow
immunoassays, please cite:

Saxena, K.; Toley, B. *Streamlining Lateral Flow Assay (LFA) Data Analysis:
A MATLAB® Live Script for Integrated Batch Image Processing and Limit of
Detection Determination.* **ChemRxiv** 2024 [Preprint].
DOI: [10.26434/chemrxiv-2024-wr3kj](https://doi.org/10.26434/chemrxiv-2024-wr3kj).

## Privacy and publication files

Images, experimental details, analysis results and other data entered into this
app are processed locally in your browser and are not uploaded to its creators
or an analysis server. No visitor analytics has been added.

The publication ZIP contains the reviewed static app and third-party licence
notices. No experimental images or private validation records are included.
When used from the GitHub repository, GitHub Actions checks the package checksum,
unpacks it and publishes it to GitHub Pages. To preview an unpacked copy locally,
serve its folder over HTTP rather than opening HTML directly as a file.

See `THIRD_PARTY_NOTICES.md` and `third-party/` inside the publication ZIP for
third-party licences. Institutional artwork remains unchanged.
