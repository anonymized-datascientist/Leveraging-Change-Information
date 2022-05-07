ASE #396 How Useful is Code Change Information for Fault Localization in Continuous Integration?

Leveraging-Change-Information is a fault dataset that contains 193 real world faults with the goal of studying fault localization in the CI context.


Projects
---------------
Leveraging-Change-Information contains a total of 192 faults across seven open source Java systems. To note that we identify the faults in JFreeChart collected from Defects4J benchmark by `Chart`, while the faults that we collected in our study take the identifier `Jfreechart`

| Identifier      | System name                |Number of faults|
|-----------------|----------------------------|---------------:|
| Fastjson        | fastjson                   |       88       |
| Lang            | lang                       |       6        |
| Math            | math                       |       22       |
| Closure         | closure                    |       41       |
| JacksonCore     | jacksoncore                |       12       |
| Time            | time                       |       5        |
| Chart           | jfreechart                 |       9        |
| Jfreechart      | jfreechart                 |       9        |

Structure
---------------
```
│
├── Chart (system identifier)
│   ├── 1 (fault id)
│   │   ├── buggy 	(coverage computed on the fault inducing commit)
│   │   ├── prior 	(coverage computed on the prior passing commit)
│   │   ├── source 	(related source and test files)
│   │   ├── inducing_changes.csv 	(code changes performed on the fault inducing commit)
│   │   └─  ...
│   └─ ...
```
