# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Data Science: Capstone Project

The Capstone Project is divided into 5 deliverables, each building on top of skills learned previously to scaffold students' learning over the entire course. Project deliverables include objectives, requirements, rubrics, and suggested resources - all of which tie into the overall competencies for this course.


### **[Capstone, Part 1: Pitch + Problem Statement][part-1]**

|Feature          |Type     |Dataset                     |Description                       |
|---              |---      |---                         |---                               |
|age              |int64    |mlb_pitch_stats_19_21, 20   |players's age                     |
|edge%            |float64  |mlb_pitch_stats_19_21, 20   |edge of zone percentage           |
|poor_weak%       |float64  |mlb_pitch_stats_19_21, 20   |poor/weak contact percentage      |
|4seam%           |float64  |mlb_pitch_stats_19_21, 20   |4seam fastball percentage thrown  |
|4seam_velo       |float64  |mlb_pitch_stats_19_21, 20   |avgerage 4seam velocity           |
|ch%              |float64  |mlb_pitch_stats_19_21, 20   |changeup percentage thrown        |
|sl%              |float64  |mlb_pitch_stats_19_21, 20   |slider percentage thrown          |
|cb%              |float64  |mlb_pitch_stats_19_21, 20   |curveball percentage thrown       |
|cu%              |float64  |mlb_pitch_stats_19_21, 20   |cutter percentage thrown          |
|throws           |object   |mlb_pitch_stats_19_21, 20   |handedness RHP: 1, LHP: 0         |

|Feature          |Type     |Dataset                     |Description                |
|---              |---      |---                         |---                        |
|player_id        |int64    |mlb_pitch_stats_19_21, 20   |player ID                  |
|last_name        |object   |mlb_pitch_stats_19_21, 20   |player last name           |
|first_name       |object   |mlb_pitch_stats_19_21, 20   |player first name          |
|year             |int64    |mlb_pitch_stats_19_21, 20   |season                     |
|age              |int64    |mlb_pitch_stats_19_21, 20   |players's age              |
|ip               |float64  |mlb_pitch_stats_19_21, 20   |number of innings pitched  |
|bf               |int64    |mlb_pitch_stats_19_21, 20   |number of innings pitched  |
|ab               |int64    |mlb_pitch_stats_19_21, 20   |number of innings pitched  |
|h                |int64    |mlb_pitch_stats_19_21, 20   |hits given up  |
|k%               |float64  |mlb_pitch_stats_19_21, 20   |strikeout percentage       |
|bb%              |float64  |mlb_pitch_stats_19_21, 20   |walk percentage            |
|ba               |float64  |mlb_pitch_stats_19_21, 20   |batting average against    |
|slg%             |float64  |mlb_pitch_stats_19_21, 20   |slugging percentage against       |
|obp%             |float64  |mlb_pitch_stats_19_21, 20   |on base percentage         |
|ops              |float64  |mlb_pitch_stats_19_21, 20   |on base plus slugging against  |
|earned_runs      |int64    |mlb_pitch_stats_19_21, 20   |earned runs   |
|era              |float64  |mlb_pitch_stats_19_21, 20   |earned run average  |
|qual_start       |int64    |mlb_pitch_stats_19_21, 20   |quality start (>= 6 ip <= 3 runs) |
|cg               |int64    |mlb_pitch_stats_19_21, 20   |complete game  |
|xba              |float64  |mlb_pitch_stats_19_21, 20   |expected ba (probability a batted ball will be a hit) |
|xslg             |float64  |mlb_pitch_stats_19_21, 20   |expected slugging percentage  |
|woba             |float64  |mlb_pitch_stats_19_21, 20   |weighted on-base average  |
|xwoba            |float64  |mlb_pitch_stats_19_21, 20   |expected weighted on-base average |
|xobp             |float64  |mlb_pitch_stats_19_21, 20   |expected on-base percentage  |
|wobacon          |float64  |mlb_pitch_stats_19_21, 20   |  |
|xwobacon         |float64  |mlb_pitch_stats_19_21, 20   |  |
|bacon            |float64  |mlb_pitch_stats_19_21, 20   |batting avgerage on contact  |
|xbacon           |float64  |mlb_pitch_stats_19_21, 20   |expected batting avgerage on contact   |
|ev_avg           |float64  |mlb_pitch_stats_19_21, 20   |average exit velocity   |
|la_avg           |float64  |mlb_pitch_stats_19_21, 20   |average LA (how high, in degrees, a ball was hit) |
|sweet_spot%      |float64  |mlb_pitch_stats_19_21, 20   |batted ball with la between 8 and 32 degrees  |
|barrel%          |float64  |mlb_pitch_stats_19_21, 20   |perfect combination of exit velocity and launch angle |
|solid_contact%   |float64  |mlb_pitch_stats_19_21, 20   |solid contact percentage  |
|poor_weak%       |float64  |mlb_pitch_stats_19_21, 20   |poor/weak contact percentage  |
|hard_hit%        |float64  |mlb_pitch_stats_19_21, 20   |exit velo > 95 mph hard hit ball percentage     |
|z_swing%         |float64  |mlb_pitch_stats_19_21, 20   |in-zone swing percentage  |
|z_swing_miss%    |float64  |mlb_pitch_stats_19_21, 20   |in-zone swing and miss percentage  |
|oz_swing%        |float64  |mlb_pitch_stats_19_21, 20   |out-zone swing percentage  |
|oz_swing_miss%   |float64  |mlb_pitch_stats_19_21, 20   |out-zone swing and miss percentage   |
|oz_contact%      |float64  |mlb_pitch_stats_19_21, 20   |out-zone contact percentage  |
|out_zone%        |float64  |mlb_pitch_stats_19_21, 20   |out_zone percentage  |
|pitch_count      |int64    |mlb_pitch_stats_19_21, 20   |pitch count   |
|z_contact%       |float64  |mlb_pitch_stats_19_21, 20   |in-zone contact percentage   |
|in_zone%         |float64  |mlb_pitch_stats_19_21, 20   |in-zone percentage  |
|edge%            |float64  |mlb_pitch_stats_19_21, 20   |edge of zone percentage  |
|whiff%           |float64  |mlb_pitch_stats_19_21, 20   |whiff percentage   |
|swing%           |float64  |mlb_pitch_stats_19_21, 20   |swing percentage   |
|gb%              |float64  |mlb_pitch_stats_19_21, 20   |ground ball percentage  |
|fb%              |float64  |mlb_pitch_stats_19_21, 20   |fly ball percentage   |
|ld%              |float64  |mlb_pitch_stats_19_21, 20   |line drive percentage   |
|po%              |float64  |mlb_pitch_stats_19_21, 20   |popup percentage   |
|throws           |object   |mlb_pitch_stats_19_21, 20   |handedness RHP: 1, LHP: 0               |
|n_pitches        |int64    |mlb_pitch_stats_19_21, 20   |number of pitches thrown        |
|4seam%           |float64  |mlb_pitch_stats_19_21, 20   |4seam fastball percentage thrown       |
|4seam_velo       |float64  |mlb_pitch_stats_19_21, 20   |avgerage 4seam velocity       |
|4seam_spinrate   |float64  |mlb_pitch_stats_19_21, 20   |avgerage 4seam spinrate       |
|4seam_hb         |float64  |mlb_pitch_stats_19_21, 20   |avgerage 4seam horizontal break        |
|4seam_vb         |float64  |mlb_pitch_stats_19_21, 20   |avgerage 4seam vertical break        |
|4seam_brk        |float64  |mlb_pitch_stats_19_21, 20   |avgerage 4seam total break        |
|4seam_velo_range |float64  |mlb_pitch_stats_19_21, 20   |4seam velocity range       |
|sl%              |float64  |mlb_pitch_stats_19_21, 20   |slider percentage thrown      |
|sl_velo          |float64  |mlb_pitch_stats_19_21, 20   |avgerage sl velocity       |
|sl_spinrate      |float64  |mlb_pitch_stats_19_21, 20   |avgerage sl spinrate         |
|sl_hb            |float64  |mlb_pitch_stats_19_21, 20   |avgerage sl horizontal break       |
|sl_vb            |float64  |mlb_pitch_stats_19_21, 20   |avgerage sl vertical break        |
|sl_brk           |float64  |mlb_pitch_stats_19_21, 20   |avgerage sl total break       |
|sl_velo_range    |float64  |mlb_pitch_stats_19_21, 20   |sl velocity range       |
|ch%              |float64  |mlb_pitch_stats_19_21, 20   |changeup percentage thrown        |
|ch_velo          |float64  |mlb_pitch_stats_19_21, 20   |avgerage ch velocity       |
|ch_spinrate      |float64  |mlb_pitch_stats_19_21, 20   |avgerage ch spinrate       |
|ch_hb            |float64  |mlb_pitch_stats_19_21, 20   |avgerage ch horizontal break       |
|ch_vb            |float64  |mlb_pitch_stats_19_21, 20   |avgerage ch vertical break        |
|ch_brk           |float64  |mlb_pitch_stats_19_21, 20   |avgerage ch total break       |
|ch_velo_range    |float64  |mlb_pitch_stats_19_21, 20   |ch velocity range       |
|cb%              |float64  |mlb_pitch_stats_19_21, 20   |curveball percentage thrown       |
|cb_velo          |float64  |mlb_pitch_stats_19_21, 20   |avgerage cb velocity       |
|cb_spinrate      |float64  |mlb_pitch_stats_19_21, 20   |avgerage cb spinrate       |
|cb_hb            |float64  |mlb_pitch_stats_19_21, 20   |avgerage cb horizontal break        |
|cb_vb            |float64  |mlb_pitch_stats_19_21, 20   |avgerage cb vertical break        |
|cb_brk           |float64  |mlb_pitch_stats_19_21, 20   |avgerage cb total break         |
|cb_velo_range    |float64  |mlb_pitch_stats_19_21, 20   |cb velocity range       |
|cu%              |float64  |mlb_pitch_stats_19_21, 20   |cutter percentage thrown       |
|cu_velo          |float64  |mlb_pitch_stats_19_21, 20   |avgerage cu velocity       |
|cu_spinrate      |float64  |mlb_pitch_stats_19_21, 20   |avgerage cu spinrate        |
|cu_hb            |float64  |mlb_pitch_stats_19_21, 20   |avgerage cu horizontal break        |
|cu_vb            |float64  |mlb_pitch_stats_19_21, 20   |avgerage cu vertical break        |
|cu_brk           |float64  |mlb_pitch_stats_19_21, 20   |avgerage cu total break        |
|cu_velo_range    |float64  |mlb_pitch_stats_19_21, 20   |cu velocity range       |


### **[Capstone, Part 2: Dataset + Data Collection][part-2]**

Use your newfound skills to source and collect the relevant data for your project. Data acquisition, transformation, and cleaning are typically the most time-consuming parts of data science projects, so don’t procrastinate!

- **Requirements**: Source and format the data for your project. Perform preliminary data munging and cleaning of the data relevant to your project goals.  Describe your data keeping the intended audience of your final report in mind
- **Format:** Table, file, or database with relevant text file or notebook description


### **[Capstone, Part 3: EDA + Preliminary Analysis][part-3]**

Begin quantitatively describing and visualizing your data. With rich datasets, EDA can go down an endless number of roads. Maintain perspective on your goals and scope your EDA accordingly. Managing your own time is a critical skill in analysis projects.  Keep notes on your approach, results, setbacks, and findings.

- **Requirements**: Perform initial descriptive and visual analysis of your data. Identify outliers, summarize risks and limitations, and describe how your EDA will inform your modeling decisions
- **Format:** Jupyter Notebook(s)


### **[Capstone, Part 4: Findings + Technical Report][part-4]**

Share your technical findings with your fellow data scientists. Explain your goals, describe modeling choices, evaluate model performance, and discuss results. Data science reporting is technical, but don’t forget that you should tell a compelling story about your data.

- **Requirements**: Summarize your goals and metrics for success, variables of interest, and removal of any outliers or data imputation. Your process description should be concise and relevant to your goals. Summarize statistical analysis, including model selection,  implementation, evaluation, and inference. Be convincing – justify all important decisions! Clearly label plots and visualizations. Include an Executive Summary
- **Format:** Jupyter Notebook(s)


### **[Capstone, Part 5: Presentation + Non-Technical Summary][part-5]**

Take your findings and share a 10 minute presentation that delivers the most important insights from your project to a non-technical audience. Tell us the most interesting story about your data. Break down your process for a novice audience. Make sure to include compelling visuals. Time is short, so be sure to practice and include only the most relevant components of your project.

- **Requirements**: Convey your goals, limits/assumptions, methods and their justification, findings, and conclusions. Define technical terms. Include graphics and visualizations
- **Format:** Interactive graphic presentation, website, or slide deck


### Approximate Due Dates

These are all subject to change!

Date | Assignment 
-----| ----------
8/31 | [Part 1][part-1]
9/10 | [Part 2][part-2]
9/22 | [Part 3][part-3]
10/1 | [Part 4][part-4]
10/4 | [Part 5][part-5]

<!--- LINKS --->

[part-1]: ./part-01/
[part-2]: ./part-02/
[part-3]: ./part-03/
[part-4]: ./part-04/
[part-5]: ./part-05/
