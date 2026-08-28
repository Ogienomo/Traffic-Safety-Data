SP FREIGHT CRASH SEVERITY — COMPANION DATA BUNDLE
==================================================
Article: "Freight Vehicle Involvement and Crash Severity in Sao Paulo State:
Evidence from Traffic-Safety Data"

FOLDERS
-------
analysis_tables/  All 16 analysis tables behind the Excel workbook:
  01_annual_series.csv          State fatal-crash series 2015-2025 (deaths, rates, truck/bus/heavy shares)
  02_severity_spectrum.csv      Severity by involvement group 2019-2025
  03_chi2_truck.csv             Chi-square: fatal outcome x truck involvement
  04_chi2_stratified.csv        Same test stratified by road type
  05_yearly_severity.csv        Fatality rate by year x truck involvement
  06_logit_fatal_crash.csv      Crash-level logistic regression (odds of fatal crash)
  07_logit_person_death.csv     Person-level logistic regression (odds of victim death)
  08_truck_crash_victims.csv    Deaths by victim mode in truck-involved fatal crashes
  09_vru_deaths.csv             VRU comparison: truck-involved vs all fatal crashes
  10_corridors.csv              Top 30 highway corridors
  11_municipalities_top50.csv   Top 50 municipalities (+ 11b_municipalities_all.csv = all 639)
  12_crash_types.csv            Crash type x truck involvement
  13_vehicle_counts.csv         Vehicles involved by type and year
  14_administration.csv         Fatal crashes by road administration
  15_der_vdm_summary.csv        DER traffic volumes (VDM) 2020-2025
  15b_der_vdm_segments_2024.csv Top DER segments by commercial traffic
  16_der_crashes_summary.csv    DER network crashes 2023-2025

ibge/            IBGE 2022 Census population (645 municipalities) + annual state estimates
der/             DER-SP open data (VDM, crashes 2023-2025, road network, Anuario 2024)

MAIN MICRODATA
--------------
The full INFOSIGA-SP microdata (1.32M crash events, 1.79M persons, 1.57M vehicles,
monthly CSVs Jan 2015 - Dec 2025) are in: INFOSIGA_microdata_consolidated_2015-2025.zip
(consolidated, analysis-ready; source: dadosabertos.sp.gov.br, CC-BY-4.0).
Original monthly files: https://dadosabertos.sp.gov.br/dataset/eventos-de-sinistro

REPRODUCIBILITY
---------------
Scripts (download, consolidation, analysis, workbook build):
  /home/z/my-project/scripts/download_infosiga.py
  /home/z/my-project/scripts/consolidate_infosiga.py
  /home/z/my-project/scripts/analyze_infosiga.py
  /home/z/my-project/scripts/summarize_der.py
  /home/z/my-project/scripts/build_workbook.py

Access date for all sources: 2026-08-26.
