# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
### REG.NO: 212223100043
### NAME : RAGUL RAAJAN T
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
<img width="934" height="721" alt="Screenshot 2025-09-20 172846" src="https://github.com/user-attachments/assets/29b00d3d-9149-408d-9af4-702803e7de39" />
<img width="1413" height="777" alt="Screenshot 2025-09-20 171718" src="https://github.com/user-attachments/assets/08aa896d-d031-46e5-8e5e-fadfae2f3e96" />
<img width="1919" height="702" alt="Screenshot 2025-09-20 144502" src="https://github.com/user-attachments/assets/5e9aceb2-c66c-45aa-aeed-5b20840ffbdc" />
<img width="1030" height="532" alt="Screenshot 2025-09-20 172055" src="https://github.com/user-attachments/assets/68dfe3d7-4650-4ef4-a0a8-7ef6f0675b90" />

<img width="1919" height="1079" alt="Screenshot 2025-09-20 144937" src="https://github.com/user-attachments/assets/6f52a826-d2c8-4852-a430-8941f52adaab" />
<img width="1441" height="937" alt="Screenshot 2025-09-20 144740" src="https://github.com/user-attachments/assets/ad0a086e-7bfa-400e-a694-74c48a405187" />

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

