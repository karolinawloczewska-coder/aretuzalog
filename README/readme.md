# Aretuzalog – Attendance Tracker

**Aretuzalog** is a personal data analytics project focused on tracking attendance, learning progress, and patterns of productivity during a data analytics bootcamp.  
It began as a simple Excel sheet but is evolving into a structured, Python-powered dashboard designed to explore, analyse and visualise personal data in real time.

![Aretuzalog Logo](/assets/images/Logo.png)

---

## Dataset Content
- The dataset represents attendance and learning activity data.
- Each sheet in the Excel file corresponds to a specific week.
- Columns represent days or sessions; a value of `1` indicates attendance.
- Data are updated manually for now and will later be loaded dynamically using Python (Pandas).

---

## Business Requirements
- Build a clean, flexible system for tracking total attendance and progress over time.  
- Automate calculation of total attendance and weekly averages.  
- Show how many sessions are required to maintain a chosen attendance level.  
- Display sessions per week and remaining sessions to the end of the course.  
- Help plan ahead and track consistency in learning habits.  

---

## Hypothesis and Validation
*Hypothesis:*  
Consistency in attendance correlates with motivation, skill growth, and improved learning outcomes.  
Learning through practice — the project will evolve as I apply new Python, data, and visualisation skills, solving challenges as they appear.

*Validation Plan:*  
Use Python (Pandas) to calculate weekly and cumulative attendance trends.  
Compare attendance consistency with periods of active engagement and task completion.  
Adjust the logic as I learn more advanced techniques during the bootcamp.

---

## Project Plan
1. Design project structure (`data/`, `scripts/`, `notebooks/`, `assets/`, `reports/`).
2. Build a static dashboard in HTML and CSS.
3. Create Python scripts to load and process Excel data.
4. Generate attendance summaries and statistics.
5. Integrate with the dashboard dynamically (in future versions).
6. Document the process and findings in this README.

---

## Mapping Business Requirements to Data Visualisations
| Business Requirement | Planned Visualisation |
|----------------------|------------------------|
| Track overall attendance | Summary metric / total counter |
| Show attendance trends | Line or area chart over time |
| Track weekly attendance | Bar chart by week |
| Forecast remaining sessions | Simple text summary / counter |

---

## Analysis Techniques Used
(Current plan — will be updated as project evolves)
- Data loading and cleaning with **pandas**
- Descriptive statistics and percentage calculations
- Simple trend analysis (attendance over time)
- Future: predictive planning based on course schedule

---

## Ethical Considerations
- Data are **strictly personal**, representing only the author’s own attendance and learning data.
- No third-party or sensitive information is included.
- Files are stored locally and shared publicly only as anonymised, non-sensitive datasets.

---

## Dashboard Design
The dashboard (`index.html`) contains:
- **Header** – project title and logo  
- **Links** – access to project README for documentation  
- **Planned Widgets:**
  - Total attendance summary
  - Weekly breakdown
  - Remaining sessions
  - Target progress indicator

---

## Unfixed Bugs
- Automatic calculation of attendance from multiple Excel sheets still in development.
- Dynamic HTML data integration not yet implemented (planned with Flask or JS).
- CSS layout will be adjusted once data widgets are added.

---

## Development Roadmap
| Phase | Focus |
|-------|--------|
| Phase 1 | Base structure, static dashboard |
| Phase 2 | Data processing scripts |
| Phase 3 | Basic statistics and visualisation |
| Phase 4 | Dynamic dashboard integration |
| Phase 5 | Forecasting and reporting |

Challenges faced so far:
- Managing focus shifts and workflow consistency.
- Learning new tools while structuring real data step by step.

---

## Deployment
(Currently local only – hosted via `python -m http.server`)

Future deployment options:
- GitHub Pages (for static HTML version)
- Streamlit / Flask app for interactive analytics

---

## Main Data Analysis Libraries
Planned / partially used:
- **pandas** – load and process Excel data  
- **openpyxl** – read/write `.xlsx` files  
- **matplotlib** – visualisations  
- **numpy** – calculations  

Example usage (to be added later in code section):
```python
import pandas as pd
df = pd.read_excel('data/Attendance_Tracker.xlsx', sheet_name='Current Week')
attendance_rate = df['attended'].sum() / len(df) * 100
print(f"Attendance: {attendance_rate:.1f}%")

---

## Content

Base README structure inspired by Code Institute Data Analytics Template.
HTML/CSS starter from Code Institute learning materials.
Logo concept (“Dagaz + Thurisaz”) designed by the author.

---

## Media

All images and icons are original or open-license.

---

## Acknowledgements

Thanks to my Bootcamp instructors and peers for ongoing feedback.

