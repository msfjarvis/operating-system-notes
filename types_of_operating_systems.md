# Types of Operating Systems

Operating Systems are classified under multiple categories depending on their scheduling and execution techniques. Some more common types of Operating Systems are as follows:

* Batch OS
* Multi-programmed OS
* Time sharing OS
* Network OS
* Distributed OS
* Real-time OS
* Network OS

## Batch OS

Batch processing is a technique in which an OS collects the programs and data together in a batch before processing starts. An OS does the following activities related to batch processing:

* The OS defines the job which has predefined sequence of commands, programs and data as a single unit.
* The OS keeps a number of jobs in the memory and executes them without manual intervention.
* Jobs are processed in the order of summation such that the first-come-first-serve paradigm is respected.
* When a job completes its execution, its memory is released and the output for the job is copied into an output spool for later printing or processing.

`// Insert diagram here`

The OS is termed as batch processing because the input data or jobs are collected into batches and set of records with similar needs and each batch is processed as a unit. The output is another batch that can be reused for computation.

* In this OS, the user does not interact directly with the computer system.
* The user prepared a job (input data) using offline devices like punch cards and submitted it to the operator.
* After some time the output appeared, consisting of the result of the program as well as a dump of the final memory and register contents for debugging.
* To speed up the processing, operators batched together jobs with similar needs and ran them through the computer as a group.
* In this execution environment, the CPU is often idle because the speed of mechanical input/output devices are much slower than the electronic devices.
* Operating system's major task was to transfer content automatically from one job to the next.
* The operating system was always resident in the memory.

### Advantages

* Batch processing is particularly useful for the operations that require the computer or a peripheral device for an extended period of time and requires very little user interaction.
* Batch processing takes much of the work of the operator to the computer.
* Increased performance as a new job gets started as soon as the previous job is finished, without manual intervention.

### Disadvantages

* Job setup was a real problem. It took a lot of time for mounting of tapes or cards.
* No interaction is possible with user while the program is being executed.
* A job could enter into an infinite loop.
* Due to lack of protection scheme, one batch job can affect the pending jobs.
* CPU remains idle during transition from one job to another.

In order to reduce the wastage of time during job transition, automatic job sequencing was developed. The first operating system, known as Resident Monitor, came into existence. Initially, Resident Monitor was invoked and then it would transfer the control to the program. When the program terminated, it would return the control to the Resident Monitor. Then control goes to the next program, then back again and so on and so forth. The Resident Monitor would automatically sequence the execution of jobs one after another.

Resident Monitor has many identifiable parts, the major one of which was the control card interpreter that was responsible for reading and carrying out instructions on the cards at the point of execution.

## Multi-programmed OS

An OS that can run multiple *programs* on a *single* processor is a multi-programmed OS.

## Time sharing OS

Operating Systems that schedule tasks based on a set quota of time and offload them when the time is up regardless of completion state are called time sharing OSes.

## Real-time OS

They are of two types, soft real-time OS and hard real-time OS.
