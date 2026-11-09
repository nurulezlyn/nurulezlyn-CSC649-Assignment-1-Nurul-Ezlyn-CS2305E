# Problem Statement

Sterile processing staff and operating theatre nurses must count surgical instruments by hand against a count sheet before a tray is assembled, and again after surgery. This manual count depends on focus and is easy to get wrong when staff are rushed, distracted or faced with many similar-looking instruments (Deol et al., 2024; Nosrati et al., 2025). A count error can go unnoticed until the tray is used, which can delay operations or, in the worst case, leave an instrument inside the patient. Lynus et al. (2026) report that retained surgical items occur in roughly 1 in 5,500 to 1 in 7,000 procedures, and Nichol et al. (2024) link instrument errors to lost chargeable operating room minutes.

## Users and stakeholders

| Group | Role |
|---|---|
| Sterile processing staff (primary user) | Prepare, supervise and validate tray contents; may upload tray images. |
| Operating theatre nurses (primary user) | Check tray contents before and after a procedure. |
| Hospital management (stakeholder) | Concerned with patient safety and process efficiency. |
| Patients (indirect beneficiary) | Benefit from safer instrument management. |

## Scope

| In scope | Out of scope |
|---|---|
| Upload one tray image (JPG or PNG), taken from overhead with good lighting. | Real-time video detection. |
| Detect, classify and count the instrument classes in the dataset. | Instruments not included in the dataset. |
| Compare counts with the tray checklist and report missing or extra instruments. | Images with heavy overlap of instruments or poor quality. |
| Dataset annotation, training and evaluation (precision, recall, mAP). | Integration with hospital systems or replacing the official count. |

The system is advisory at the prototype stage. The final decision is made by trained personnel.

Sources are listed in [references](references.md).
