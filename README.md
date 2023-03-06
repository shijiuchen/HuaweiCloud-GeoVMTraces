# Regionless orchestration datasets
## Overview
The Regionless orchestration datasets is published by Huawei Group. By providing standard data sets for orchestration and scheduling of computing resources, it can help researchers better study and train scheduling algorithms. We are open source based on Apache License V2.0. Please follow the open source protocol when using datasets.

The dataset contains the usage data of 20 tenants in 17 regions during 122 days. Each tenant has a separate table. Each table consists of four fields: Date, Region id, VM type id used by the tenant, and number of VM cores that the tenant is using at the current time.

Such as:
|  Date   | Region id  | VM type id | Using VM cores |
|  ----  | ----  | ----  | ----  | 
| 1 00:00:00  | r8 | v3 | 272 |
| 1 00:00:00  | r1 | v1 | 30 |
| 1 00:10:00  | r1 | v3 | 32 |
| 1 00:10:00  | r4 | v5 | 1568 |

There are some explainations of the dataset for avoiding users' confusion.
1. A tenant may use more regions or VM types which are not included in the trace.
2. For the data of a tenant, the region and VM type without record at a specific date represents the tenant does not use it at this date.
3. For the data of a tenant, if there's no record during a specific day, it means the tenant does not use VMs at this day.

We encourage anyone to use the datasets for study or research purposes, and if you had any question when using the datasets, please file an issue on Github. Filing an issue is recommanded as the discussion would help all the community. Note that the more clearly you ask the question, the more likely you would get a clear answer.

We are open source based on Apache License V2.0. When using datasets, please follow the open source protocol, and cite our paper.

```BibTeX
@inproceedings{shi2022characterizing,
  title={Characterizing and orchestrating VM reservation in geo-distributed clouds to improve the resource efficiency},
  author={Shi, Jiuchen and Fu, Kaihua and Chen, Quan and Yang, Changpeng and Huang, Pengfei and Zhou, Mosong and Zhao, Jieru and Chen, Chen and Guo, Minyi},
  booktitle={Proceedings of the 13th Symposium on Cloud Computing},
  pages={94--109},
  year={2022}
}
```
## Papers using regionless orchestration datasets
Jiuchen Shi, Kaihua Fu, Quan Chen, Changpeng Yang, Pengfei Huang, Mosong Zhou, Jieru Zhao, Chen Chen and Minyi Guo. Characterizing and orchestrating VM reservation in geo-distributed clouds to improve the resource efficiency[C]//Proceedings of the 13th Symposium on Cloud Computing. 2022: 94-109.

## LISCENCE
Licensed under the Apache License V2.0.

## Future works
More datasets will be released in future.

## Download dataset
**[The download link.](https://gitee.com/HuaweiCloudDeveloper/huaweicloud-regionless-dataset)**
