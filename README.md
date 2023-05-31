# Khronos-dataset

Data are provided to the review process for paper Khronos: A Real-Time Indexing Framework for Time Series Databases on Large-Scale Performance Monitoring Systems.

The data contains the following four datasets:

(1) ASI: Time series data corpus collected from a container scheduling system.
(2) HI: Time series data corpus collected from a resource scheduling system.
(3) IG: Time series data corpus collected from an online graph engine.
(4) TPP: Time series data corpus collected from a search and recommendation platform.

The demo directory contains three demo segments of the above datasets, while the dataset directory contains the segments for 3 consecutive days.

The segment is an [ORC](https://github.com/apache/orc) file, which can be parsed by [tool](https://github.com/apache/orc/blob/main/tools/src/FileContents.cc). Each segment has 3 columns. The first column is the seriesKey (including one metric and tag key and tag value pairs), while the second and third columns are the start and end timestamps of the corresponding time series, respectively. Note that data is partially desensitized to preserve privacy.
