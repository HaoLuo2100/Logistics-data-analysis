客户B的数据共包含8个数据文件，下面来依次介绍：
1. address_B.txt
本文件内容与原始数据集中的“客户需求分析-地址数据(客户B).txt”内容相同。
2. waybill_B.txt
本文件内容与原始数据集中的“客户需求分析-运单数据(客户B).txt”内容相同。
3. address_B_easy.txt
本文件内容基于address_B.txt筛选获得。
筛选标准是只筛选出卸货点在同一个城市的运单，将相应地址数据放在本文件中。
数据格式与address_B.txt相同。
4. loadCity_B.txt
本文件内容基于waybill_B.txt筛选获得。
筛选标准是筛选出作为提货点的城市名称。
数据格式是（提货省，提货市）
5. loadCity_B_pro.txt
本文件内容基于waybill_B.txt筛选获得。
筛选标准是筛选出作为提货点的省名称。
数据格式是（提货省）
6. UnloadCity_B.txt
本文件内容基于waybill_B.txt筛选获得。
筛选标准是筛选出作为卸货点的城市名称。
数据格式是（卸货省，卸货市）
7. UnloadCity_B_pro.txt
本文件内容基于waybill_B.txt筛选获得。
筛选标准是筛选出作为卸货点的省名称。
数据格式是（卸货省）
8. result_B.csv
本文件内容基于时间序列的统计算法获得。
算法核心是统计提货点和卸货点之间按月份的方数时间序列和吨数时间序列。
数据格式是（提货省，卸货省，方数时间序列，吨数时间序列）
