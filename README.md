# Clean BLS County Level Employment Data

This file cleans employment and unemployment data by County from the U.S. Bureau of Labor Statistics (BLS). These data are known as Local Area Unemployment (LAU) statistics. The raw text files are not easy to immediately manipulate, so this cleaning file produces a "long format" .csv file for ease of use.

# Getting Started

BLS LAU data are available monthly from 1990-2017, and can be found at: <https://download.bls.gov/pub/time.series/la/>. In order to run this cleaning code, download the following files from the above link to the same folder as this script:

- la_area.txt
- la_data_0_CurrentU90_94.txt
- la_data_0_CurrentU95_99.txt
- la_data_0_CurrentU00_04.txt
- la_data_0_CurrentU05_09.txt
- la_data_0_CurrentU10_14.txt
- la_data_0_CurrentU15_19.txt

# Code output

The code produces a .csv file with the following columns.

- FIPS code
- State
- County name
- Year
- Month
- Employment (level)
- Labor force (level)
- Unemployment (level)
- Unemployment rate

If all data from 1990-2017 is used, the resulting .csv file is approximately 60mb in size.

# Prerequisites

The script requires 'Python' along with the 'pandas' library.

# Running the code

The code can be run directly from the command line via: ''' python BLS_LAU_County.py '''

# Author

- James Graham (NYU, 2017)

# License

This project is licensed under the MIT License.
