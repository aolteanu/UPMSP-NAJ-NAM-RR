# UPMSP-NAJ-NAM-RR

Benchmarks for the unrelated parallel machine scheduling with job and machine acceptance and renewable resource allocation.

Two folders containing the comma-separated files for problems instances of different sizes can be found:

## small-instances

This folder contains 20 problem instances for all configurations combining the following problem parameters:

* the number of jobs, $n \in \{10,20,30,40,50\}$;
* the number of machines, $m \in \{10,20\}$;
* the number of resource types, $k = 5$.

## large-instances

This folder contains 20 problem instances for all configurations combining the following problem parameters:

* the number of jobs, $n \in \{100,200,300,400,500\}$;
* the number of machines, $m = 50$;
* the number of resource types, $k = 10$.

## Format

Each problem instance is split into multiple files. All files pertaining to a problem instance have the following prefix: P`n`-`m`-`k`-`index`_`comp`, where n, m, k correspond to the previous parameters while index corresponds to the instance index (from 1 to 20 in our case).

The `comp` part indicates the type of data that can be found in the file:

* "a", the resource type requirements for each job, as a matrix of $n\times k$ of $\{0,1\}$ values;
* "deadline", the deadlines of the jobs, as a matrix of $1\times n$ of numerical values;
* "due", the due dates of the jobs, as a matrix of $1\times n$ of numerical values;
* "fc", the fixed costs of the jobs, as a matrix of $1\times n$ of numerical values;
* "l", the number of available resources of each type, as a matrix of $1\times k$ of integer values;
* "mwtm", the minimum renting time of machines, as a matrix of $1\times m$ of numerical values;
* "p", the profits of the jobs, as a matrix of $1\times n$ of numerical values;
* "pc", the penalty costs of the jobs, as a matrix of $1\times n$ of numerical values;
* "rcm", the rental costs of machines per unit of time, as a matrix of $1\times m$ of numerical values;
* "rcr", the rental costs of resource types per unit of time, as a matrix of $1\times k$ of numerical values;
* "t", the processing time of jobs on machines, as a matrix of $n\times m$ of numerical values;
* "tc", the tardiness costs of the jobs, as a matrix of $1\times n$ of numerical values;
* "trcj", the transfer costs of jobs to machines (or setup cost), as a matrix of $m\times n$ of numerical values;
* "trcr", the transfer costs of resources between machines, as a matrix of $1\times k$ of numerical values;
* "trtj", the transfer times of jobs to machines (or setup times), as a matrix of $m\times n$ of numerical values;
* "trtr", the transfer times of resources between machines, as a matrix of $1\times k$ of numerical values;

## License

This project is under MIT license. Please see the [LICENSE](LICENSE) file for more information.
