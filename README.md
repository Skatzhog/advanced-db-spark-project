# LA Crimes — Advanced Database Topics Project (NTUA, 2025)

## Overview
Semester team project for the *Advanced Database Topics* course of the Electrical & Computer Engineering Department, National Technical University of Athens.

The project focuses on large-scale data processing and analytical querying using **Apache Spark** (and HDFS where applicable) on an AWS SageMaker–based cluster provided by the course.  
We analyze Los Angeles crime data (2010–present) and auxiliary datasets (census, income, police stations) to answer a set of predefined analytical queries.

## Technologies
- Apache Spark (RDD, DataFrame & SQL APIs)
- Hadoop / HDFS
- Python (PySpark)
- AWS SageMaker (course-provided environment)

## Environment
The code is designed to run on the preconfigured AWS environment provided by the instructors.  
It can be replicated on a custom cluster with:
- A Spark cluster
- HDFS (or an equivalent distributed filesystem)
- Python and Java properly configured on all nodes

## Repository Structure
- `*.ipynb`: Jupyter notebooks implementing each query
- `Documents/`: Query descriptions, assumptions, and discussion of results
- `Utils/`: Auxiliary datasets and helper files

## Usage
Each notebook corresponds to a specific query of the assignment and contains:
- Data loading and preprocessing
- Query implementation
- Execution results and timing measurements

Open and run the notebooks sequentially in a Spark-enabled Jupyter environment.

## Datasets
| Dataset | Source |
|-------|--------|
| LA Crime Data (2010–2019) | https://data.lacity.org/Public-Safety/Crime-Data-from-2010-to-2019/63jg-8b9z |
| LA Crime Data (2020–Present) | https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-Present/2nrs-mtv8 |
| 2020 Census Blocks | https://data.lacounty.gov/maps/lacounty::2020-census-blocks |
| Census Block Fields | `utils/Datasets/LA_Census_Blocks_2020_fields.csv` |
| Median Household Income (ZIP, 2021) | http://www.laalmanac.com/employment/em12c_2021.php |
| LAPD Police Stations | https://geohub.lacity.org/datasets/lahub::lapd-police-stations |
| Race & Ethnicity Codes | `utils/Datasets/RE_codes.csv` |
| MO Codes | https://data.lacity.org/api/views/63jg-8b9z/files/e14442b9-a6b8-4531-83f3-f7ba980b1377 |

## Authors
- Nikitas Panagiotopoulos — https://github.com/Skatzhog  
- Fotis Daskalakos — https://github.com/fotisd16
