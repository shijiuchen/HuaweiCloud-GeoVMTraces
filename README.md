# HuaweiCloud-GeoVMTraces
# Overview of Geo-distributed VM Request Traces
This repository includes the VM request traces of the top 20 tenants in 4 months of 2021 in Huawei Cloud. Our traces have new features with Geo-distributed Clouds and large tenant characeteristics. In the traces, the datacenters are widely distributed into 17 regions, which contains the north, east, south of China, and parts of the southeast Asia regions. Moreover, the traces contain 12 different types of flavors with different performance in our Cloud. 

In Huawei Cloud, we have utilized the motivation analyzed from this trace dataset to develop our Geo-distributed resource reservation and scheduling strategy named _ROS_ into our cloud scheduler. We have conducted a data analysis on the trace and introduce the design of _ROS_ in a paper, named "**Characterizing and Orchestrating VM Reservation in
Geo-distributed Clouds to Improve the Resource Efficiency**", which will be published in SoCC’22. We would encourage anybody who uses this trace to cite our paper.

So far, the internal data privacy protection process of Huawei Cloud has not been completed, so the data open-sourced work is on progress. We will strive to open-source the trace data in the next few months.
