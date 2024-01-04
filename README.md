# MARS-data

## Description

This repository contains data organized in multiple levels of folders, comprising .txt files and images of histograms. The data is structured to provide insights and analysis through visualizations.

## Folder Structure

The data is organized into the following folder structure:

```
Bench-in-loop/
│
├── Characterisation/
│   ├── Characterisation_(benchName)_(data)/
│   │   ├── file_1.txt
│   │   ├── file_2.txt
│   │   ├── ...
│   │   └── Summary.xlsx
│   └── ...
│
├── Dense_Linear_Algebra/
│    ├── (Allocation_Method)/
│    │   ├── (Bench_folder)
│    │   │   ├── (metric_measured).txt
│    │   │   ├── (metric_measured)_histogram.png
│    │   │   └── ...
│    │   └── ...
│    ├── ...
│    └── DWARF_Summary.xlsx
│
├── Graph_Traversal/
│    ├── (Allocation_Method)/
│    │   ├── (Bench_folder)
│    │   │   ├── (metric_measured).txt
│    │   │   ├── (metric_measured)_histogram.png
│    │   │   └── ...
│    │   └── ...
│    ├── ...
│    └── DWARF_Summary.xlsx
│   
└── (Other DWARFS)...
```

## Usage

Explore the data and visualizations to gain insights about the conclusions of "Embedded GPU Memory Allocation Regarding Safety".
Characterisation folder contains text files with all data gathered from a static analysis of the code and an Excel file which summarize al raw data.
The next folders contains text documents of temporal analysis organised as explained before, a first level which contains the DWARF evaluated and an Excel file, a second level with the allocation method for each DWARF with text files and its histograms. Please notice that this files had no header, this was convenient for faster coding when parsing data for extracting mean and standard deviation values.

```
exeTime.txt files has this header
 Start (ns)  Duration (ns)        Name        Result  CorrID   Pid     Tid    T-Pri  Thread Name
 ----------  -------------  ----------------  ------  ------  ------  ------  -----  -----------

 While the other metrics use:
Time (%)  Total Time (ns)  Instances   Avg (ns)     Med (ns)    Min (ns)   Max (ns)   StdDev (ns)   Category                            Operation                        
 --------  ---------------  ---------  -----------  -----------  ---------  ---------  -----------  -----------  ---------------------------------------------------------

On the first one we calculate the mean and standard deviation of all executions by adding "Start" and "Duration".
On the second case they are calculated using the fourth column "Average".
```

## Acknowledgments

- Mention any contributors or resources that you found helpful.


