# Stage2: Parallelized Concept Induction and Label Hypothesis Generation(ECII tool)

**Required Inputs:**

1) config_files/neuron_<neuron_id>.config

     (_Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage1_Results/config_files_)
   
     These config files have been produced as a result of Stage 1.

# Steps to run this script local system on IntelliJ:

To run concept induction sript: 

-e config_file_name.config

Example config file: https://github.com/Samatha1994/ExAI_related_documents/blob/main/set6-initial_score_hybrid.config

Example command: -e set6-initial_score_hybrid.config

**Expected Outputs:** 

1) config_files/	neuron_<neuron_id>_results_ecii_V2.txt

    (_Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage1_Results/config_files_)


# Steps to Run the Script on BeoCat:

**Bash file name:** job_stage2.sh

**Bash Script:** https://github.com/Samatha1994/Bash_scripts/blob/main/job_stage2.sh

**Bash Command to kick off the job:** sbatch job_stage2.sh

**Bash command to check the status of the job:**

sacct --format=JobID,JobName,State,ReqMem,MaxRSS,Start,End,TotalCPU,Elapsed,NCPUS,NNodes,NodeList --jobs= <job_id>

**Log file:** my_job_output_<job_id>.txt (_Path: /homes/samatha94/_)

**Bash Command to cancel the job:** scancel job_id
