# Initial Use-case Benchmarking Data

This repository contains datasets and information of the source code used for the initial benchmarking results of the use-cases on available hardware, as reported in Deliverable 5.1. 

Details of the source code for the different use-cases is provided below:

## Virtual Screening Workflow
The scripts, information and data necessary to execute the Apache Airflow-based molecular docking virtual screening workflow presented in Section 3 of Deliverable 5.1 are available as part of a separate git repository, at https://github.com/opencube-horizon/autodock-workflow.

## iPIC3D Plasma Simulation Workflow
For the PIC plasma simulation workflow, presented in Section 4 of Deliverable 5.1, the source code can be found in the git repository https://github.com/opencube-horizon/pic-workflow.

## CloudSuite Benchmark 
The scripts used to obtain the data in the `cloudsuite-data` subdirectory are in the repository https://github.com/opencube-horizon/cloudsuite-scripts/tree/M12.
For CloudSuite, the OpenCUBE fork at https://github.com/opencube-horizon/cloudsuite/tree/M12 was used, which contains some fixes.

## Meteorological Post-processing
The baseline performance metrics for the meteorological cloud post-processing benchmarks, presented in Section 6 of Deliverable 5.1, are the result of running the PProc workflow (https://github.com/opencube-horizon/pproc-workflow) and Polytope benchmark (https://github.com/opencube-horizon/polytope-benchmark) on ECMWF's Kubernetes Cluster.

Both benchmarks can be run by executing the `run-benchmark.sh` script and the results of the initial runs can be found in the `pproc-data` and `polytope-data` subdirectories. For the different runs inside the `pproc-data`, we record the time required to perform data retrieval and archival as well as computation time for expensive tasks. The results in `polytope-data` record the time required to perform the extraction of different features from meteorological data, such as a timeseries or flight path. 

## IFS Dwarfs
The two IFS dwarfs used in OpenCUBE are the cloud microphysics kernel CLOUDSC, available at 
https://github.com/ecmwf-ifs/dwarf-p-cloudsc,
and the spherical transforms library, which can be found at
https://github.com/ecmwf-ifs/ectrans.


Both projects come with a benchmarking driver, which is used for the establishment of performance results. The drivers are compiled by default when the dwarfs are compiled.

# License

All code is under the Apache 2 license.
All images are under the CC-BY 4.0 license.
