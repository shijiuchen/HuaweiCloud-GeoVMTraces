# Huawei Cloud Geo-distributed VM Traces
# Overview of Geo-distributed VM Request Traces
This repository includes the VM request traces of the top 20 tenants in 4 months (122 days) of 2021 in Huawei Cloud. Our traces have new features with Geo-distributed Clouds and large tenant characeteristics. In the traces, the datacenters are widely distributed into 17 regions, which contains the north, east, south of China, and parts of the southeast Asia regions. Moreover, the traces contain 29 different flavors (VM typtes) with different performance in our Cloud. 

Every tenant has a record file, which is named "ALLDATE_xxx.csv". In the file, there are 4 fields in each row, which represents the "record time", "region", "flavor", and "CPU cores usage", respectively. The "record time" is ordered from the 1st day's 0' clock to the 122nd day's 24 0'clock, i.e., from "1 00:00:00" to "122 23:50:00". The fields of "region" and "VM type" are reordered into "r1-r17" and "v1-v12", respectively.

## Trace Notes
There are some explainations of the traces for avoiding users' confusion.
1. A tenant may use more regions or flavors which are not included in the trace.
2. For the data of a tenant, the region and flavor without record at a specific time point represents the tenant does not use it at this time point.
3. For the data of a tenant, if there's no record at a specific day, it means the tennat does not use the VMs at his day.

## Huawei Cloud Deployment
In Huawei Cloud, we have utilized the motivation analyzed from this trace dataset to develop our Geo-distributed resource reservation and scheduling strategy named _ROS_ into our cloud scheduler. We have conducted a data analysis on the trace and introduce the design of _ROS_ in a paper, named [Characterizing and Orchestrating VM Reservation in
Geo-distributed Clouds to Improve the Resource Efficiency](https://dl.acm.org/doi/pdf/10.1145/3542929.3563490), which was published in SoCC’22. This paper is a collaboration between SJTU-EPCC and Huawei Cloud. We would encourage anybody who uses this trace to cite our paper.

```BibTeX
@inproceedings{shi2022characterizing,
  title={Characterizing and orchestrating VM reservation in geo-distributed clouds to improve the resource efficiency},
  author={Shi, Jiuchen and Fu, Kaihua and Chen, Quan and Yang, Changpeng and Huang, Pengfei and Zhou, Mosong and Zhao, Jieru and Chen, Chen and Guo, Minyi},
  booktitle={Proceedings of the 13th Symposium on Cloud Computing},
  pages={94--109},
  year={2022}
}
```

**So far, the internal data privacy protection process of Huawei Cloud has not been completed. We will open-source the trace data by December, 2022.**
