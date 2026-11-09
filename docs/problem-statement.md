# Problem Statement

The staff in sterile processing and operating rooms must first tallied the surgical instruments according to the count sheet before assembling the instruments tray. They then have to check the instruments once again after the surgery by doing the manual verification of the count. This counting is based on focus and is susceptible to errors when one counts the items that are in a hurry, distracted or face confusion with numerous similar-looking instruments (Deol et al., 2024; Nosrati et al., 2025). Violation of the count may go unnoticed until the analyzer is going to be used, and this may lead to delays in operations, or result in the presence of a surgical instrument in the patient after surgery has been completed (Lynus et al., 2026). According to Lynus et al. (2026), the occurrence of surgical equipment retention is equivalent to about 1 in 5,500 and 1 in 7,000 surgical procedures, while Nichol et al. (2024) have noted that the instrument errors in the surgical instruments have an impact on the chargeable operation time minutes. 

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
