# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report

<img width="944" height="746" alt="491898046-5075b4de-599d-4a93-a762-336d61778fd0" src="https://github.com/user-attachments/assets/7ccb2ec8-e2cf-4001-8a08-cbe238831282" />

<img width="1920" height="1080" alt="491898063-0dc4a16d-6087-418a-bcc1-a793ec08c70e" src="https://github.com/user-attachments/assets/22b48f93-ae80-4e59-bf3d-341e10d49d1b" />

<img width="1920" height="1080" alt="491898066-df722e77-4be8-4eec-aea2-13ff8c821bb8" src="https://github.com/user-attachments/assets/8abd5d4d-55e7-4ab5-bcff-736cea30b509" />

<img width="1920" height="1080" alt="491898095-713dfb4b-0f34-4f81-8d39-b9a4c539f2a5" src="https://github.com/user-attachments/assets/84dd5d48-8275-4722-af61-4008c9d01221" />

<img width="1920" height="1080" alt="491898104-073e3188-196a-49b3-bf09-1e31851b23ab" src="https://github.com/user-attachments/assets/9c584c40-22c7-4f23-a6fa-917b9b4d7f3d" />

<img width="1920" height="1080" alt="491898110-3730692c-d571-4c1c-ba2f-9b456d6d7072" src="https://github.com/user-attachments/assets/e906540d-ef57-47aa-867b-e28152dd1ce7" />

<img width="1920" height="1080" alt="491898129-06253722-6c7e-488a-a089-e61836836fa1" src="https://github.com/user-attachments/assets/b491603c-4012-4c9c-b4e9-9a551fe61820" />

<img width="1920" height="1080" alt="491898137-606a8fc7-ae5c-4493-afa9-38e2254797ac" src="https://github.com/user-attachments/assets/cdf546ff-e7a2-441a-97f5-660db59d5cd6" />

<img width="1920" height="1080" alt="491898145-4f34846d-3131-47b0-9bb0-371a385cf136" src="https://github.com/user-attachments/assets/82cab1ba-ccd6-4152-b431-9204a06e29be" />

<img width="1920" height="1080" alt="491898153-7bab635b-135d-4f5d-a106-5a2d8bd15a1d" src="https://github.com/user-attachments/assets/1dd4fe07-9ae2-4733-9567-06dfa0cac459" />










## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.
