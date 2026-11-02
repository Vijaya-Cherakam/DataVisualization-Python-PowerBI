Optimizing Clinical TFL Review with Python and Power BI: A Reproducible Workflow to Reduce QC Time and Improve Traceability
This project demonstrates a hybrid quality-control (QC) workflow for clinical trial Tables, Listings, and Figures (TLFs), integrating:
- SAS — generation of production Analysis Data Model (ADaM) datasets and TFL outputs.
- Python — independent QC validation and comparison checks.
- Microsoft Power BI — interactive visualization of QC results and discrepancies.
The workflow is designed to complement established clinical statistical programming processes by making selected review checks more reproducible, transparent, and easier to investigate. It does not replace validated production programming, independent review, or required regulatory quality controls.
Objectives
- Demonstrate an independent Python-based QC approach for selected clinical TFL review checks.
- Organize QC findings in a structured format for review.
- Use Power BI to help reviewers explore discrepancies and patterns.
- Improve traceability by documenting the inputs, checks, and outputs used in the workflow.
- Share a reproducible example that can be adapted using synthetic or appropriately authorized data.
Workflow
1. SAS generates the ADaM datasets and production TFL outputs.
2. Python scripts read the relevant input data and perform independent QC checks.
3. The Python QC results identify potential differences or discrepancies for review.
4. Power BI visualizes the QC results to support investigation and traceability.
SAS production outputs
ADaM datasets and TFL outputs
        |
Python independent QC checks
        |
Structured QC results / discrepancies
       |
Power BI review and visualization
Repository contents
The repository may contain Python scripts, input examples, Power BI files, and supporting documentation. Refer to the files currently present in the repository for the implemented scope.

Example command referenced by this project:
python python/pilot project.py
How to run
1. Prerequisites
- Python installed and available from your command line.
- The project files cloned or downloaded locally.
- The input datasets and file paths expected by the scripts.
- Power BI Desktop, if you want to open and explore the Power BI report.
2. Install Python dependencies
From the repository root, run:
pip install -r requirements.txt
For a cleaner environment, you may create and activate a virtual environment before installing dependencies.
3. Run the demographic QC script
From the repository root, run:
python python/ pilot project.py
Review the script and its comments for the expected input locations, required variables, output locations, and any project-specific configuration. Other scripts, if present, may have their own run instructions.
4. Review results in Power BI
If a Power BI report is included, open it in Power BI Desktop and configure its data source to use the appropriate QC output files. Review the displayed results against the underlying QC outputs and source data.
Reproducibility and traceability
For each QC run, users should be able to identify:
- The input datasets and TFL outputs used.
- The script and software versions used.
- The checks performed and their assumptions.
- The location and format of generated QC results.
- Any discrepancies, exclusions, or manual review decisions.
When extending the project, document changes to derivations, comparison rules, input requirements, and expected outputs. Keep example data and expected results small enough for reviewers to reproduce the demonstration.
Data privacy and responsible use
Do not commit confidential, identifiable, or restricted clinical-trial data to this repository. Use synthetic data or data that is explicitly authorized for public distribution. Before publishing, inspect spreadsheets, datasets, notebooks, reports, screenshots, commit history, and metadata for protected health information (PHI), personally identifiable information (PII), sponsor/CRO confidential information, credentials, and proprietary content.
This project is an illustrative workflow and is not, by itself, a validated clinical system. Any use in a regulated or production environment requires appropriate validation, governance, documented procedures, and qualified review.
Limitations
- The checks implemented are limited to those present in the repository scripts.
- QC results depend on the quality, structure, and suitability of the input data.
- A discrepancy is a review finding, not necessarily proof that a production output is incorrect.
- Power BI visualizations support exploration; they do not independently establish statistical or clinical correctness.
Citation
If you use or adapt this project, please cite the version you used. GitHub can display citation information when the repository includes a valid CITATION.cff file. For a persistent, version-specific citation, archive a formal release with Zenodo and add the DOI to this section after it has been issued.
Author
Vijaya Lakshmi Cherakam
- GitHub: https://github.com/Vijaya-Cherakam
- ORCID: https://orcid.org/0009-0004-1245-2618
Contributions and feedback
Suggestions, bug reports, and improvements are welcome. Please use GitHub Issues to describe the use case, steps to reproduce a problem, expected behavior, and (where possible) a small synthetic example. Do not include confidential or identifiable clinical information in issues or pull requests.
License
Add a license only after confirming that you have the rights to license all code and materials in this repository. Until a license is included, users should not assume that they have permission to reuse, modify, or redistribute the contents.
