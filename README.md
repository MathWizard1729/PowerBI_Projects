# PowerBI Projects

A home for my Power BI projects.

## Cybersecurity breaches

- `Cybersecurity breaches Project.pbix`: the Power BI report.
- `Cyber Security Breaches.csv`: its data source, about 1,050 rows. Columns include the covered entity,
  type of breach, where the information was held, individuals affected, breach start and end dates,
  branch, department and country, and an estimate of the data stolen (GB).

The report has two pages, each filterable by country, breach type and branch or department:

- **Branch Analysis**: total breaches, open versus closed breaches by branch, estimated stolen data (GB)
  by branch, breaches by type, and a gauge of the average days until a breach ended.
- **Department Analysis**: the same measures broken down by department.

The data model splits the CSV into Branch, Department, Country and Types of Breach tables, with the
calculations in a `DAX Measures` table (Total, Open and Closed Breaches, Estimate Stole Data (GBs),
Avg Breach End days).

To open it, install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (Windows) and open the
`.pbix` file. If the data fails to load, point the query's source at the CSV in this folder.
