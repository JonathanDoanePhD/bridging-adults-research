# Verified public datasets (direct download, no account)

Links were checked on the date shown. "Used in" points to projects whose `data/sources.csv`
holds the exact file links. Check license terms before publishing.

| Dataset | What it covers | Level | Direct link (or listing page) | Checked | Used in |
|---|---|---|---|---|---|
| Census SAIPE 2022 | Child poverty, median household income | County | https://www2.census.gov/programs-surveys/saipe/datasets/2022/2022-state-and-county/est22all.xls | 2026-11-13 | 01 |
| CDC/ATSDR Social Vulnerability Index 2022 | 16 barrier measures + 4 themes | County | https://svi.cdc.gov/Documents/Data/2022/csv/states_counties/SVI_2022_US_county.csv | 2026-11-13 | 01 |
| Opportunity Insights county / tract outcomes | Adult outcomes by parent income, race, gender | County, tract | https://www2.census.gov/ces/opportunity/county_outcomes_simple.csv (`tract_outcomes_simple.csv`) | 2026-11-13 | 01 |
| Opportunity Insights covariates | Place characteristics | County, tract | https://opportunityinsights.org/wp-content/uploads/2018/12/cty_covariates.csv | 2026-11-13 | 01 |
| Social Capital Atlas | Economic connectedness, exposure, friending bias, clustering, civic orgs | County, ZIP, high school, college | https://data.humdata.org/dataset/social-capital-atlas (license: redistribute with license; no endorsement; no re-identification) | 2026-11-13 | 01, 02 |
| College Mobility Report Cards | Low-income-to-high-income mobility by college | College | https://opportunityinsights.org/wp-content/uploads/2018/04/mrc_table2.csv (scripted download may get 403; plain curl works) | 2026-11-14 | 04 |
| IRS Exempt Organizations BMF | Every registered nonprofit with NTEE category code | Organization | https://www.irs.gov/pub/irs-soi/eo1.csv (eo2-eo4) | 2026-11-13 | 01 |
| Census ZCTA-county relationship 2020 | ZIP area to county overlap | ZCTA | https://www2.census.gov/geo/docs/maps-data/data/rel2020/zcta520/tab20_zcta520_county20_natl.txt | 2026-11-13 | 01 |
| Census cartographic boundaries 2022 | County shapes for maps | County | https://www2.census.gov/geo/tiger/GENZ2022/shp/cb_2022_us_county_20m.zip | 2026-11-13 | 01 |
| National Survey of Children's Health 2024 | Adult mentor item, flourishing, adversity, school engagement | Child (parent report) | https://www2.census.gov/programs-surveys/nsch/datasets/2024/nsch_2024_topical_Stata.zip | 2026-11-13 | 02 |
| PISA 2022 student questionnaire | Belonging, self-efficacy, teacher support, achievement; ~80 countries | Student | https://webfs.oecd.org/pisa2022/STU_QQQ_SPSS.zip (682 MB; school file: `SCH_QQQ_SPSS.zip`) | 2026-11-13 | 02 phase 2 (planned) |
| EDFacts graduation rates (Urban Institute bulk CSV) | 4-yr graduation rates by school and subgroup, 2010-2019 | School | https://educationdata.urban.org/csv/edfacts/schools_edfacts_grad_rates_2018.csv (year = year the school year begins, verified; license ODC-By 1.0) | 2026-11-13 | 02 |
| NCES Common Core of Data 2018-19 | Free/reduced lunch (file 033), enrollment (file 052); cp1252 encoding | School | https://nces.ed.gov/ccd/Data/zip/ccd_sch_033_1819_l_1a_091019.zip, ..._052_1819_l_1a_091019.zip | 2026-11-13 | 02 |
| CDC Youth Risk Behavior Survey 2023 | School connectedness, adult support, risk behaviors | Student (HS) | https://www.cdc.gov/yrbs/files/2023/XXH2023_YRBS_Data.dat + 2023XXH-SAS-Input-Program.sas (fixed-width; the .zip is an Access file) | 2026-11-13 | 02 |

| College Scorecard (most recent, institution) | Net price by income, Pell share, completion, earnings by family income | College | https://ed-public-download.scorecard.network/downloads/Most-Recent-Cohorts-Institution_11022026.zip (file name changes with each release; see collegescorecard.ed.gov/data) | 2026-11-14 | 04 |
| Census Gazetteer counties 2022 | County internal points (lat/lon) | County | https://www2.census.gov/geo/docs/maps-data/data/gazetteer/2022_Gazetteer/2022_Gaz_counties_national.zip | 2026-11-14 | 04 |
| American Time Use Survey 2003-2023 | Diary minutes by activity, who was present, family income | Person-day | https://www.bls.gov/tus/datafiles/atusresp-0323.zip (also atusact, atuswho, atuscps, atusrost) | 2026-11-14 | 05 |
| Civil Rights Data Collection 2017-18 and 2015-16 | Counselors, psychologists, social workers, nurses, officers; chronic absence; discipline | School | https://civilrightsdata.ed.gov/assets/ocr/docs/2017-18-crdc-data.zip, .../2015-16-crdc-data.zip (2015-16 IDs need rebuilding: see 06) | 2026-11-14 | 06 |
| NCES Common Core of Data 2017-18 | Free/reduced lunch (033), directory incl. school type (029) | School | https://nces.ed.gov/ccd/Data/zip/ccd_sch_033_1718_l_1a_083118.zip, ..._029_1718_w_1a_083118.zip | 2026-11-14 | 06 |
| BLS earnings and unemployment by education | Median weekly earnings, unemployment by attainment | National | https://www.bls.gov/emp/tables/unemployment-earnings-education.htm | 2026-11-14 | 07 |
| NSF Award Search API | Award abstracts, program, obligated dollars, place of performance (drop PI/PO personal fields) | Award | https://api.nsf.gov/services/v1/awards.json?fundProgramName=AISL&dateStart=01/01/2014&dateEnd=12/31/2024&rpp=25&offset=1 (keyless; 25 per page; program filter matches words loosely, so filter exact names locally; bulk download page now redirects) | 2026-11-19 | 09 |
| USAspending API | Federal grants by Assistance Listing: award descriptions, recipients, county totals by place of performance | Award / county | https://api.usaspending.gov/api/v2/search/spending_by_geography/ and .../spending_by_award/ (keyless POST JSON; filter by program_numbers) | 2026-11-19 | 09 |
| IRS Form 990 e-file data | Mission, program descriptions and expenses, revenue, staff and volunteer counts (parse only those elements; never Part VII or schedules naming people) | Organization-year | https://apps.irs.gov/pub/epostcard/990/xml/2024/index_2024.csv and .../2024_TEOS_XML_NNA.zip (12 zips, about 2.8 GB; file names use upper-case "A" even when the index says "a") | 2026-11-20 | 10 |
| Census county adjacency 2023 | Neighboring counties | County | https://www2.census.gov/geo/docs/reference/county_adjacency/county_adjacency2023.txt | 2026-11-20 | 10 |
| O*NET 30.0 database | Task statements and importance, required education, job zones (CC BY 4.0) | Occupation / task | https://www.onetcenter.org/dl_files/database/db_30_0_text.zip | 2026-11-25 | 11 |
| ACS table-based summary files | Any ACS table as a pipe-delimited file, no API key (e.g. B24121 earnings by detailed occupation, C24010 county occupation mix) | Nation to county | https://www2.census.gov/programs-surveys/acs/summary_file/2023/table-based-SF/data/1YRData/acsdt1y2023-b24121.dat (5YRData for counties; labels in .../documentation/ACS20231YR_Table_Shells.txt) | 2026-11-25 | 11 |
| Census 2018 occupation code list and crosswalk | Census occupation codes to SOC 2018 | Occupation | https://www2.census.gov/programs-surveys/demo/guidance/industry-occupation/2018-occupation-code-list-and-crosswalk.xlsx | 2026-11-25 | 11 |
| NCES CIP 2020 to SOC 2018 crosswalk | College programs to occupations | Program | https://nces.ed.gov/ipeds/cipcode/Files/CIP2020_SOC2018_Crosswalk.xlsx | 2026-11-25 | 11 |
| College Scorecard field of study | Earnings and debt by program and credential, incl. Pell national medians | Program | https://ed-public-download.scorecard.network/downloads/Most-Recent-Cohorts-Field-of-Study_10152026.zip (file name changes with releases) | 2026-11-25 | 11 |
| Eloundou et al. (2024) GPTs are GPTs labels | Task-level human and GPT-4 exposure labels (MIT) | Task | https://raw.githubusercontent.com/openai/GPTs-are-GPTs/main/data/full_labelset.tsv | 2026-11-25 | 11 |

## Ruled out (needs an account or column picking)

PSID, NLSY (NLS Investigator), Add Health and other ICPSR holdings, IPUMS, HUD ZIP crosswalk,
the Data Resource Center version of NSCH (use the Census files above instead), Kaggle (needs a
login to download). The Census data API now requires a registered key (use the table-based summary
files instead). bls.gov refused downloads from this environment as of 2026-11-25 (HTTP 403), so
BLS files (OEWS, projections, ATUS) may need to be fetched elsewhere.
