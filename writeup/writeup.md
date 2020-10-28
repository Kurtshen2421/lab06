Writeup question #1: Consider a serial vector with 15 entries (0.0, 0.1, 0.2, ..., 1.3, 1.4). If you ran this code with 4 processes, which data entries would end up on rank 0? on rank 1? on rank 2? on rank 3?

Writeup question #3: Copy the output of your slurm file.

```
Job ran on: ca114
Tue Oct 27 23:07:21 EDT 2020: Start loop
-----------------------------------
Number of processes: 1
WARNING: serial norm was 2.495505e+03 but parallel norm was 0.000000e+00
----------------------------------
-----------------------------------
Number of processes: 2
--------------------------------------------------------------------------
A system call failed during shared memory initialization that should
not have.  It is likely that your MPI job will now either abort or
experience performance degradation.

  Local host:  ca114
  System call: open(2)
  Error:       Permission denied (errno 13)
--------------------------------------------------------------------------
Rank 0 got parallel norm 0.000000e+00
WARNING: serial norm was 2.495505e+03 but parallel norm was 0.000000e+00
[ca114:13470] 1 more process has sent help message help-opal-shmem-mmap.txt / sys call fail
[ca114:13470] Set MCA parameter "orte_base_help_aggregate" to 0 to see all help / error messages
----------------------------------
-----------------------------------
Number of processes: 4
--------------------------------------------------------------------------
A system call failed during shared memory initialization that should
not have.  It is likely that your MPI job will now either abort or
experience performance degradation.

  Local host:  ca114
  System call: open(2)
  Error:       Permission denied (errno 13)
--------------------------------------------------------------------------
Rank 0 got parallel norm 0.000000e+00
Rank 1 got parallel norm 0.000000e+00
Rank 2 got parallel norm 0.000000e+00
WARNING: serial norm was 2.495505e+03 but parallel norm was 0.000000e+00
[ca114:13526] 3 more processes have sent help message help-opal-shmem-mmap.txt / sys call fail
[ca114:13526] Set MCA parameter "orte_base_help_aggregate" to 0 to see all help / error messages
----------------------------------
-----------------------------------
Number of processes: 6
Rank 0 got parallel norm 0.000000e+00
Rank 1 got parallel norm 0.000000e+00
Rank 2 got parallel norm 0.000000e+00
Rank 3 got parallel norm 0.000000e+00
Rank 4 got parallel norm 0.000000e+00
WARNING: serial norm was 2.495505e+03 but parallel norm was 0.000000e+00
----------------------------------
-----------------------------------
Number of processes: 8
--------------------------------------------------------------------------
A system call failed during shared memory initialization that should
not have.  It is likely that your MPI job will now either abort or
experience performance degradation.

  Local host:  ca114
  System call: open(2)
  Error:       Permission denied (errno 13)
--------------------------------------------------------------------------
Rank 1 got parallel norm 0.000000e+00
Rank 2 got parallel norm 0.000000e+00
Rank 3 got parallel norm 0.000000e+00
Rank 0 got parallel norm 0.000000e+00
Rank 4 got parallel norm 0.000000e+00
Rank 5 got parallel norm 0.000000e+00
Rank 6 got parallel norm 0.000000e+00
WARNING: serial norm was 2.495505e+03 but parallel norm was 0.000000e+00
[ca114:13796] 3 more processes have sent help message help-opal-shmem-mmap.txt / sys call fail
[ca114:13796] Set MCA parameter "orte_base_help_aggregate" to 0 to see all help / error messages
----------------------------------
-----------------------------------
Number of processes: 10
--------------------------------------------------------------------------
A system call failed during shared memory initialization that should
not have.  It is likely that your MPI job will now either abort or
experience performance degradation.

  Local host:  ca114
  System call: open(2)
  Error:       Permission denied (errno 13)
--------------------------------------------------------------------------
Rank 3 got parallel norm 0.000000e+00
Rank 2 got parallel norm 0.000000e+00
Rank 1 got parallel norm 0.000000e+00
Rank 5 got parallel norm 0.000000e+00
Rank 6 got parallel norm 0.000000e+00
Rank 7 got parallel norm 0.000000e+00
Rank 4 got parallel norm 0.000000e+00
Rank 0 got parallel norm 0.000000e+00
WARNING: serial norm was 2.495505e+03 but parallel norm was 0.000000e+00
Rank 8 got parallel norm 0.000000e+00
[ca114:14021] 3 more processes have sent help message help-opal-shmem-mmap.txt / sys call fail
[ca114:14021] Set MCA parameter "orte_base_help_aggregate" to 0 to see all help / error messages
----------------------------------
Tue Oct 27 23:07:34 EDT 2020: End loop
```