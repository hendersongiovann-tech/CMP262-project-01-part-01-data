# CMP 262 Data Exploration and Visualization

**Due: Module 6 · Worth: 100 points**

Use Python to identify **four findings that could help CCM attract more students to computing classes**. Continue from your completed Data Cleaning project.

## GitHub Starter Repository

[Open the starter repository](https://github.com/ahedhli12/CMP262-Project-01-Part-01-Data-DV)

### Getting Started

1. Open the starter repository.
2. Select **Use this template → Create a new repository**. If that button is unavailable, select **Fork → Create fork** to make your own copy.
3. Choose your personal GitHub account as the owner.
4. Name your repository **LastName-FirstName-CMP262-Data-DV**.
5. Set the repository to **Public**, then create it.
6. Clone **your own** repository and open it in Visual Studio Code.
7. Copy your completed **majors_survey_cleaned.csv** and **nonmajors_survey_cleaned.csv** from Part 1 into this repository's **data** folder. Keep the originals in Part 1 unchanged.
8. Open **DataVisualization.ipynb** and select your Python kernel.
9. Run the provided import and loading cells. Confirm that both files load.
10. Complete all four finding sections and the final summary.
11. Run and test all notebook cells.
12. Complete **AI-Use-Report.md**.
13. Save, commit, and push your work to GitHub.
14. Submit your public repository link through Blackboard Ultra.

**Important:** Clone your own newly created repository, not the instructor's starter repository. This starter intentionally contains no survey CSV files or completed findings.

## Copy and load your cleaned data

Use the cleaned files from your completed [Part 1 Data Cleaning project](https://github.com/ahedhli12/CMP262-Project-01-Part-01-Data-Cleaning-), not the original survey exports.

Your files should be organized like this:

- DataVisualization.ipynb
- AI-Use-Report.md
- data/majors_survey_cleaned.csv
- data/nonmajors_survey_cleaned.csv

The notebook already includes this starter code:

```python
# Load tools for data tables and charts.
import pandas as pd
import matplotlib.pyplot as plt

# Read the two cleaned CSV files.
majors = pd.read_csv("data/majors_survey_cleaned.csv")
nonmajors = pd.read_csv("data/nonmajors_survey_cleaned.csv")
```

Copying the files places them in your project. Running read_csv() loads their contents into pandas tables. If you see FileNotFoundError, check the folder, spelling, and filename. Open the repository folder in VS Code and run the notebook from that project.

## Your task

For each of your **four different findings**, include:

1. **Question:** What do you want to learn about recruitment, student interests, or communication?
2. **Code:** Analyze the relevant data with pandas. Comment the important steps.
3. **Chart:** Create at least one appropriate chart with a clear title and labels where applicable.
4. **Evidence:** Describe the result using actual counts or percentages from your output.
5. **Recommendation:** Explain how CCM could use the result to attract students.

Use Markdown cells for your questions, explanations, and recommendations. End with a short summary identifying your most useful recommendation and a limitation of your analysis.

### Questions to consider

- Which groups express interest in another computing class?
- How did students hear about their computing classes?
- What interests do non-computing majors have in computing?
- What might encourage students in computer literacy courses to take another computing class?

These are starting points. Choose four useful questions that your actual columns can answer. Inspect each file's column names; the two surveys may ask different questions.

### Which chart should I use?

| Your question | Chart | Simple example |
|---|---|---|
| Compare categories | Bar chart | Compare the number of students in different majors |
| Compare categories between groups | Grouped bar chart | Compare interest responses for two student groups |
| Show ranges of one numeric measure | Histogram | Count students within ranges of study hours, if available |
| Compare two numeric measures | Scatter plot | Look for an association between two numeric responses |
| Show a few categories as shares of one total | Pie chart | Show Yes, No, and Maybe shares for a single-response question |
| Follow values in a meaningful order | Line chart | Show enrollment across years, only if the data supports it |

You do not need every chart type. Choose the chart that answers each question. Do not create a time trend from data that has no time sequence.

### Analyze carefully

- Compare percentages as well as counts when groups have different sizes; report the group sizes.
- Explain how you treated missing responses and what total a percentage uses.
- Check whether a question allows multiple selections. Those responses may not add to 100% and may not suit a pie chart.
- Support conclusions with your output. A survey pattern does not prove cause and effect.
- Keep source cleaned CSV files unchanged.

## GitHub Submission

Your repository must contain:

- **DataVisualization.ipynb** with four findings, charts, commented code, and Markdown explanations
- **AI-Use-Report.md**
- **data/majors_survey_cleaned.csv**
- **data/nonmajors_survey_cleaned.csv**

Save your notebook. Restart the kernel and select **Run All** to check that your work runs in order without errors. Save again so the final outputs appear in your notebook.

Run these commands one at a time:

```bash
git status
git add .
git commit -m "Complete data exploration and visualization project"
git push
```

Open your repository on GitHub and verify the latest notebook, chart outputs, AI report, and cleaned CSV files.

## Blackboard Ultra Submission

Blackboard Ultra is the official submission location. Submit the link to your public GitHub repository there.

**Uploading your work to GitHub alone does not count as submitting the assignment.**
