Tool for gathering blocks and replicas meta data from HDFS.

Build project:

```
bin/compile
```

Usage:

``` 
bin/run <path> [<max_number_of_blocks_to_print>]
```

Example output:

```
[dlanza@itrac1505 hdfs-meta]$ bin/run /user/hloader/SCADAR/SURVEY_F3_LOAD.db/eventhistory_00100001 2

Showing metadata for: hdfs://p01001532067275.cern.ch/user/hloader/SCADAR/SURVEY_F3_LOAD.db/eventhistory_00100001
	isDirectory: true
	isFile: false
	isSymlink: false
	encrypted: false
	length: 0
	replication: 0
	blocksize: 0
	modification_time: Tue Mar 15 13:48:08 CET 2016
	access_time: Thu Jan 01 01:00:00 CET 1970
	owner: hloader
	group: supergroup
	permission: rwxr-xr-x

Collecting block locations...
Collected 269 locations.

16/03/17 17:41:56 INFO Configuration.deprecation: dfs.data.dir is deprecated. Instead, use dfs.datanode.data.dir
Data directories and disk ids
  DiskId: 0  Directory: FILE:/data01/hadoop/hdfs/data
  DiskId: 1  Directory: FILE:/data1/hadoop/hdfs/data
  DiskId: 2  Directory: FILE:/data10/hadoop/hdfs/data
  DiskId: 3  Directory: FILE:/data11/hadoop/hdfs/data
  DiskId: 4  Directory: FILE:/data12/hadoop/hdfs/data
  DiskId: 5  Directory: FILE:/data13/hadoop/hdfs/data
  DiskId: 6  Directory: FILE:/data14/hadoop/hdfs/data
  DiskId: 7  Directory: FILE:/data15/hadoop/hdfs/data
  DiskId: 8  Directory: FILE:/data16/hadoop/hdfs/data
  DiskId: 9  Directory: FILE:/data17/hadoop/hdfs/data
  DiskId: 10  Directory: FILE:/data18/hadoop/hdfs/data
  DiskId: 11  Directory: FILE:/data19/hadoop/hdfs/data
  DiskId: 12  Directory: FILE:/data2/hadoop/hdfs/data
  DiskId: 13  Directory: FILE:/data20/hadoop/hdfs/data
  DiskId: 14  Directory: FILE:/data21/hadoop/hdfs/data
  DiskId: 15  Directory: FILE:/data22/hadoop/hdfs/data
  DiskId: 16  Directory: FILE:/data23/hadoop/hdfs/data
  DiskId: 17  Directory: FILE:/data24/hadoop/hdfs/data
  DiskId: 18  Directory: FILE:/data25/hadoop/hdfs/data
  DiskId: 19  Directory: FILE:/data26/hadoop/hdfs/data
  DiskId: 20  Directory: FILE:/data27/hadoop/hdfs/data
  DiskId: 21  Directory: FILE:/data28/hadoop/hdfs/data
  DiskId: 22  Directory: FILE:/data29/hadoop/hdfs/data
  DiskId: 23  Directory: FILE:/data3/hadoop/hdfs/data
  DiskId: 24  Directory: FILE:/data30/hadoop/hdfs/data
  DiskId: 25  Directory: FILE:/data31/hadoop/hdfs/data
  DiskId: 26  Directory: FILE:/data32/hadoop/hdfs/data
  DiskId: 27  Directory: FILE:/data33/hadoop/hdfs/data
  DiskId: 28  Directory: FILE:/data34/hadoop/hdfs/data
  DiskId: 29  Directory: FILE:/data35/hadoop/hdfs/data
  DiskId: 30  Directory: FILE:/data36/hadoop/hdfs/data
  DiskId: 31  Directory: FILE:/data37/hadoop/hdfs/data
  DiskId: 32  Directory: FILE:/data38/hadoop/hdfs/data
  DiskId: 33  Directory: FILE:/data39/hadoop/hdfs/data
  DiskId: 34  Directory: FILE:/data4/hadoop/hdfs/data
  DiskId: 35  Directory: FILE:/data40/hadoop/hdfs/data
  DiskId: 36  Directory: FILE:/data41/hadoop/hdfs/data
  DiskId: 37  Directory: FILE:/data42/hadoop/hdfs/data
  DiskId: 38  Directory: FILE:/data43/hadoop/hdfs/data
  DiskId: 39  Directory: FILE:/data44/hadoop/hdfs/data
  DiskId: 40  Directory: FILE:/data45/hadoop/hdfs/data
  DiskId: 41  Directory: FILE:/data46/hadoop/hdfs/data
  DiskId: 42  Directory: FILE:/data47/hadoop/hdfs/data
  DiskId: 43  Directory: FILE:/data48/hadoop/hdfs/data
  DiskId: 44  Directory: FILE:/data5/hadoop/hdfs/data
  DiskId: 45  Directory: FILE:/data6/hadoop/hdfs/data
  DiskId: 46  Directory: FILE:/data7/hadoop/hdfs/data
  DiskId: 47  Directory: FILE:/data8/hadoop/hdfs/data
  DiskId: 48  Directory: FILE:/data9/hadoop/hdfs/data

16/03/17 17:41:57 WARN DistributedFileSystemMetadata: list of data nodes could not be got from API (requieres higher privilegies).
16/03/17 17:41:57 WARN DistributedFileSystemMetadata: getting datanode list from configuration file (may contain data nodes which are not active).

 === Distribution along nodes and disks ===

DiskId                   0 0 0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 1 1 2 2 2 2 2 2 2 2 2 2 3 3 3 3 3 3 3 3 3 3 4 4 4 4 4 4 4 4 4
                         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 Unknown   Count     Average
Host
itrac1508.cern.ch        0 = 0 = 0 = = = = 0 0 = 0 = 0 = = 0 = = + = = = + + = = = = = 0 = = + = = = = = 0 = = = = = = = = 0         77        1
itrac1512.cern.ch        0 = + = = = 0 = = 0 0 = 0 = = = 0 = 0 = = = = 0 = = = 0 = 0 = 0 + = = = = = = = 0 + = = = = = = = 0         69        1
lxfsrb53a07.cern.ch      0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0         0         0
lxfsrb53a04.cern.ch      0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0         0         0
p05153074365419.cern.ch  0 = = = = = 0 = = = 0 0 0 = 0 = = 0 0 = = 0 = 0 0 0 = 0 = 0 = 0 0 0 0 = 0 0 0 = 0 = = 0 0 = 0 = = 0         29        0
itrac1502.cern.ch        0 = = 0 = 0 0 = 0 = 0 = 0 = 0 0 = = = 0 0 = 0 = = + + = = = = = = 0 0 = = = 0 0 0 0 = 0 = = 0 = 0 0         39        0
itrac1501.cern.ch        0 = = = 0 = = = = 0 = = = = = 0 + + = = = = = = 0 = = = = = = = + = = = = 0 = = = = + = = = = = 0 0         106       2
itrac1507.cern.ch        0 = = 0 = 0 0 = = 0 0 = 0 = = = = = 0 = = + = = + = = = = = = = 0 = 0 = = 0 = = 0 = = 0 + = = = = 0         66        1
itrac1509.cern.ch        0 0 = 0 = = 0 = = 0 = = = 0 = 0 = 0 = = = = 0 0 = 0 = = = = = 0 0 = 0 = = 0 0 = 0 0 = 0 = 0 0 = 0 0         33        0
lxfsrk39a01.cern.ch      0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0         0         0
itrac1504.cern.ch        0 0 = = = = = = = 0 = = 0 = = = = 0 = 0 = = = 0 = = = 0 = = = = = 0 0 = 0 = 0 = = = = 0 = = = = 0 0         56        1
itrac1510.cern.ch        0 = 0 0 = 0 0 0 = = = 0 0 = = 0 = = = 0 = = = 0 = 0 0 = = = 0 0 0 0 0 0 = = 0 = = 0 = = = 0 + = = 0         37        0
itrac1506.cern.ch        0 0 0 = 0 = 0 = = 0 0 0 = 0 = = = = = 0 = = = = 0 = = = = 0 = = = 0 = = = = 0 + = = + + + = = = 0 0         68        1
p05153074600927.cern.ch  0 0 = 0 0 0 0 0 = 0 = 0 0 = = 0 = 0 = = = 0 = 0 = = = 0 = 0 0 0 0 0 0 0 = 0 0 = = 0 = 0 0 = = = 0 0         26        0
itrac1503.cern.ch        0 = = = = = 0 0 0 = = 0 = = 0 0 = 0 + = = = = = = = = 0 = = = = = 0 0 = = = = = = = = 0 = = = = = 0         61        1
itrac1511.cern.ch        0 = = = = = 0 = = = 0 0 = 0 = = 0 = = 0 0 = = 0 = + = = = = = 0 = = = = = = 0 + = = = = 0 = = = 0 0         64        1
itrac1505.cern.ch        0 0 = = 0 0 + = = 0 0 = = 0 0 = 0 0 = = = 0 = 0 0 = = 0 = = = = 0 0 = = = 0 = = 0 = = 0 = + = = 0 0         42        0

Leyend
  0: no blocks in this disk
  +: #blocks is more than 20% of the avergae of blocks per disk of this host
  =: #blocks is aproximatilly the avergae of blocks per disk of this host
  +: #blocks is less than 20% of the avergae of blocks per disk of this host
  
 === Metadata of blocks and replicass ===

Block (0) info:
	Offset: 0
	Length: 268435456
	No cached hosts
	Hosts:
		Replica (0):
			Host: itrac1507.cern.ch
			Location: FILE:/data30/hadoop/hdfs/data (DiskId: 24)
			Name: 128.142.210.206:1004
			TopologyPaths: /0513_R-0050/RL05/128.142.210.206:1004
		Replica (1):
			Host: itrac1503.cern.ch
			Location: FILE:/data2/hadoop/hdfs/data (DiskId: 12)
			Name: 128.142.210.232:1004
			TopologyPaths: /0513_R-0050/RL17/128.142.210.232:1004
		Replica (2):
			Host: itrac1504.cern.ch
			Location: FILE:/data34/hadoop/hdfs/data (DiskId: 28)
			Name: 128.142.210.236:1004
			TopologyPaths: /0513_R-0050/RL17/128.142.210.236:1004

Block (1) info:
	Offset: 268435456
	Length: 268435456
	No cached hosts
	Hosts:
		Replica (0):
			Host: itrac1507.cern.ch
			Location: FILE:/data19/hadoop/hdfs/data (DiskId: 11)
			Name: 128.142.210.206:1004
			TopologyPaths: /0513_R-0050/RL05/128.142.210.206:1004
		Replica (1):
			Host: itrac1509.cern.ch
			Location: FILE:/data7/hadoop/hdfs/data (DiskId: 46)
			Name: 128.142.210.237:1004
			TopologyPaths: /0513_R-0050/RL21/128.142.210.237:1004
		Replica (2):
			Host: itrac1512.cern.ch
			Location: FILE:/data25/hadoop/hdfs/data (DiskId: 18)
			Name: 128.142.210.235:1004
			TopologyPaths: /0513_R-0050/RL21/128.142.210.235:1004

16/03/17 17:41:57 WARN DistributedFileSystemMetadata: Not showing more blocks because limit has been reached
```