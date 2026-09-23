# CIP-B105-CS4_Morris_Worm_c11.dfit2617295
CIP-B105-CS4 Morris Worm Controlled Investigation – SEED Labs nano-internet (Lessons 22–27). Process, port, hash &amp; timeline analysis. Student: Mary Ekwughaonu (c11.dfit2617295)
# CIP-B105-CS4 – Morris Worm Controlled Investigation

**Student:** Mary Ekwughaonu  
**Registration Number:** c11.dfit2617295  
**Module:** CIP-B105-CS4 (ICDFA – Second Semester)  
**Submission Date:** 24 September 2026  

---

## Overview

This repository contains the complete documentation for the controlled Morris Worm investigation performed inside the isolated SEED Labs Docker nano-internet (Lessons 22–27).

The investigation followed a strict educational scope:
- Historical analysis of the 1988 Morris Worm
- Clear distinction between the original worm and the simplified SEED training implementation
- Pre-infection baseline on host `as151h-host_0`
- Post-infection process, port, hash and timestamp analysis
- Final integrated timeline and professional conclusion

**No live malware files (`worm.py` / `badfile`) are included in this repository** for security and policy reasons. All findings are documented through reports, process listings, port evidence, cryptographic hashes and timestamps.

---

## Repository Structure

```
CIP-B105-CS4_Morris_Worm/
├── README.md
├── Reports/
│   ├── Lesson_22_Report_Mary_Ekwughaonu_Morris_History.docx
│   ├── Lesson_23_Report_Mary_Ekwughaonu_NanoInternet_Baseline.docx
│   ├── Lesson_24_Report_Mary_Ekwughaonu_Morris_Worm_Process.docx
│   ├── Lesson_25_Report_Mary_Ekwughaonu_Morris_Worm_Ports.docx
│   ├── Lesson_26_Report_Mary_Ekwughaonu_Morris_Worm_Hashes_Timestamps.docx
│   ├── Lesson_27_Report_Mary_Ekwughaonu_Morris_Worm_Integrated_Timeline.docx
│   └── CIP-B105-CS4_c11.dfit2617295_Mary_Ekwughaonu_Morris_Worm_Main_Report.docx
├── Evidence/
│   ├── baseline_process_list.txt          (optional)
│   ├── post_infection_process_list.txt    (optional)
│   ├── listening_ports.txt                (optional)
│   └── hashes.txt                         (optional)
└── Screenshots/                           (optional – add if you have them)
```

---

## Key Findings Summary

| Stage              | Evidence                                      | Confidence |
|--------------------|-----------------------------------------------|----------|
| Clean Baseline     | Only `./server` listening on TCP 9090         | HIGH     |
| Infection          | New processes: `worm.py` + `nc`               | HIGH     |
| Communication      | New listening port: TCP 9999 (owned by nc)    | HIGH     |
| Integrity          | SHA-256 / MD5 of worm artefacts recorded      | HIGH     |
| Chronology         | File drop → execution → listener activation   | HIGH     |
| Overall Conclusion | Controlled infection successfully demonstrated and contained | HIGH |

---

## Important Notes

1. This work was performed exclusively inside the authorised SEED Docker nano-internet.
2. No external systems were targeted.
3. The training implementation is a simplified educational model and is **not** identical to the original 1988 Morris Worm.
4. Actual malware files (`worm.py`, `badfile`) have been deliberately excluded from this public repository.

---

## How to Verify the Work

An examiner can:
- Review the individual Lesson 22–27 reports
- Review the consolidated Main Report (`CIP-B105-CS4_..._Main_Report.docx`)
- Cross-check the process, port, hash and timestamp evidence against the integrated timeline

---

**Mary Ekwughaonu**  
c11.dfit2617295  
International Cybersecurity & Digital Forensics Academy (ICDFA)
