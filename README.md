# Stage2: Parallelized Concept Induction and Label Hypothesis Generation(ECII tool)

**Required Inputs:**

config_files/neuron_.config    (Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage1_Results/config_files)

**Expected Outputs:** 

config_files/	neuron_<neuron_id>_results_ecii_V2.txt    (Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage1_Results/config_files)



Bash file name: job_stage2.sh

Bash Command to kick off the job: sbatch job_stage2.sh

Bash command to check the status of the job:

sacct --format=JobID,JobName,State,ReqMem,MaxRSS,Start,End,TotalCPU,Elapsed,NCPUS,NNodes,NodeList --jobs= <job_id>

Log file: my_job_output_<job_id>.txt (Path: /homes/samatha94/)

Bash Command to cancel the job: scancel job_id
