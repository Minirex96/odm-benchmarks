[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

# ODM Benchmarks


This repository is a part of the [ODM](https://github.com/OpenDroneMap) project and is dedicated to benchmark sample datasets found in the [ODMData](https://github.com/OpenDroneMap/ODMdata) repository and a few other thrid party sources, to better understand the behavioural characterists of ODM. 

OpenDroneMap benchmarking data is summarized in the following pages:

* View benchmark data [organized by dataset](./data-parsed/by-dataset.md) (Markdown)
* View benchmark data [organized by ODM version](./data-parsed/by-version.md) (Markdown)
* View benchmark [raw data](./data/benchmarks.csv) (CSV)

## Datasets for Benchmarking

Preferred datasets for benchmarking at this time are:

* Brighton Beach (18 photos)
* Toledo (87 photos)
* Wietrznia (225 photos)
* Shitan (493 photos)

These and many other sample datasets are indexed at the [ODMData repository](https://github.com/OpenDroneMap/ODMdata). 

## How to Contribute Benchmarks

This section provides instructions for contributing to the ODM Benchmarks project.

* **Review Previous Benchmarks** - You can have a look at previous benchmarks which is found in the `benchmarks.csv` file, located in the `data` directory to understand various things such as for example, figuring out which dataset has been benchmarked lesser than in comparision to other datasets.

* **Select a desired Dataset** - Choose one of the datasets of your choice which is listed in the table seen above. Links to download the dataset is provided in the same. 

* **Run the Dataset** - Create a new task in ODM and process the images.

* **Verify the results** - Ensure that the task completed successfully by viewing the maps and models generated

* **Submit Your Results** - Open the `benchmarks.csv` file and look at the header for each of the column and note the desired information required before submitting and edit the csv file. Submissions are accepted Via a Pull Request or you can choose to post your results on the [ODM community forum](https://community.opendronemap.org/t/odm-benchmark-data/3877). A table is given below to explain the structure of the CSV.

| Attribute          | Explanation                                                          | Example                                         |
| ------------------ | -------------------------------------------------------------------- | ----------------------------------------------- |
| ID                 | Benchmark Number                                                     | 1                                               |
| DATASET            | Dataset Name                                                         | Toledo                                          |
| PROCESSING_TIME    | Time taken to Process The dataset                                    | 1h 9m                                           |
| PROCESSING_SUCCESS | Confirm If process was successful                                    | Y                                               |
| ERROR_TYPE         | Mention error if any occured                                         | -                                               |
| RAM_SIZE           | Size of RAM allocated                                                | 16 GB                                           |
| RAM_CLOCK_SPEED    | RAM Frequency of the Machine                                         | 2133 MT/s                                       |
| CPU_TYPE           | Make and model of the CPU                                            | Intel i5                                        |
| CPU_CLOCK_SPEED    | Clock Speed of the CPU                                               | 2.3 Ghz                                         |
| CPU_NUM_CORES      | Number of Cores of the CPU                                           | 4                                               |
| STORAGE_TYPE       | Storage Type of the system. HDD/SSD/NVME                             | SSD                                             |
| OS                 | Operating System of the Machine                                      | Ubuntu 18.04                                    |
| VM_TYPE            | Virtual Machine on which ODM is running on                           | Docker                                          |
| ODM_VERSION        | Version of ODM Used to Benchmark                                     | 1.3.1                                           |
| ODM_CLUSTER        | Delcaration of usage of Cluster ODM                                  | N                                               |
| CONFIG_NAME        | Mention of the Configuration in which the dataset is being processed | Default                                         |
| CONFIG_RESIZE      | mention of image size if images are being resized                    | 2048 px                                         |
| CONFIG_OTHER       | Other Configurations made that are worth mentioning                  | -                                               |
| TEST_DATE          | Date of Test                                                         | 2020-03-07                                      |
| TEST_BY            | Information of the individual who tests the data                     | [Corey Snipes](https://github.com/coreysnipes/) |
| INCLUDE_IN_SUMMARY | Check if Data has been included in summary                           | Y                                               |
| NOTES              | Additional Notes                                                     | -                                               |

## Queries and Contributions

* **Questions and Doubts** - Any queries you may have can be posted in the [ODM community forum](https://community.opendronemap.org/t/odm-benchmark-data/3877).

* **Contributing new Benchmark Data** - If you have benchmark data to share, See [this page](https://github.com/OpenDroneMap/odm-benchmarks/blob/master/CONTRIBUTING.md) for details on contributing.

## License

[MIT License](LICENSE)
