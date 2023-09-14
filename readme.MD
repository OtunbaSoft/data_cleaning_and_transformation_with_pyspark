# Data Cleaning & Transformation with PySpark

## Description
<p>Rheeza Clinics & Pharmaceuticals conducted a research on Naproxen - a drug that has been claimed to normalize the blood pressure of teens and young adults. The trial was carried out in three of their clinic branches on over 2000 individuals of mixed genders from ages 14 - 22 between February and May 2021.</p>
<p>This trial involved two groups - The in-active (Placebo) and active (Naproxen) groups to test the effect of the actual drug (Naproxen). Records of all procedures were kept; and extracted from the storage for the ML Engineers to develop algorithms for the next stages of the experiment.</p>
<p>It was discovered that the dataset needed some Engineering to be performed on it for easier access by the Clinicians & ML Engineers.</p>

## Tools
<ul>
    <li>Python</li>
    <li>Pyspark</li>
</ul>


## Initial Schema
root<br><ul>
 <li>|-- ageofparticipant: long (nullable = true)</li>
 <li>|-- clinician: struct (nullable = true)</li>
 <li>|    |-- branch: string (nullable = true)</li>
 <li>|    |-- name: string (nullable = true)</li>
 <li>|    |-- role: string (nullable = true)</li>
 <li>|-- drug_used: string (nullable = true)</li>
 <li>|-- experimentenddate: string (nullable = true)</li>
 <li>|-- experimentstartdate: string (nullable = true)</li>
 <li>|-- noofhourspassedatfirstreaction: long (nullable = true)</li>
 <li>|-- result: struct (nullable = true)</li>
 <li>|    |-- conclusion: string (nullable = true)</li>
 <li>|    |-- sideeffectsonparticipant: string (nullable = true)</li>
</ul>

 ## Final Schema
 root<br><ul>
 <li>|-- age_of_participant: long (nullable = true)</li>
 <li>|-- clinic_branch: string (nullable = true)</li>
 <li>|-- branch: string (nullable = true)</li>
 <li>|-- head_clinician: string (nullable = true)</li>
 <li>|-- assistants_role: string (nullable = true)</li>
 <li>|-- drug_used: string (nullable = true)</li>
 <li>|-- experiment_end_date: string (nullable = true)</li>
 <li>|-- experiment_start_date: string (nullable = true)</li>
 <li>|-- hours_passed_at_first_reaction: long (nullable = true)</li>
 <li>|-- result: struct (nullable = true)</li>
 <li>|-- conclusion: string (nullable = true)</li>
 <li>|-- observed_side_effects: string (nullable = true)</li>
 </ul>