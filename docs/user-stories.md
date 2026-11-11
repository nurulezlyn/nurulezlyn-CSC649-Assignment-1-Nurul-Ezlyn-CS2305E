# User Stories and Acceptance Criteria

## US1: Image upload and detection
**Linked requirements:** FR1, FR2, FR3, FR4, FR5, FR12

As a sterile processing technician, I want to upload a picture of an instrument tray, which will indicate the supported instruments, so that I can verify the tray without searching for each object manually.

**Acceptance criteria**
1. When a readable JPG or PNG image is uploaded, the system displays the image with all the accepted detections, including class labels and bounding boxes. 
2. If a corrupted or unsupported file is uploaded, the system will show an error, denying any detection outcome.


## US2: Instrument counts
**Linked requirements:** FR6, FR7, FR12

As an operating theatre nurse, I want  to know the amount of detections for each type of instrument, so that I can compare the items in a tray with the expected quantity of items.

**Acceptance criteria**
1. The output will list all the types of instruments present in the image and their detected quantity for each type.
2. The count of detection for each type corresponds to the number of bounding boxes recognized for instrument type.


## US3: Checklist reconciliation
**Linked requirements:** FR8, FR9, FR10, FR11, FR13

As a sterile processing technician, I want the detected counts to be inspected against the checklist of a given tray,so that I can note down the missing or extra prior to the tray advancing to the next stage in the workflow.

**Acceptance criteria**
1. If the checklist anticipates 3 scissors and 3 forceps, while the detector shows a count of 3 scissors and 2 forceps, then 1 forceps is marked as missing in the result.
2. If the detector counts 4 scissors in comparison to an expected number of 3, then 1 scissor is registered as extra in the result. 
3. If all of the figures match, the system indicates that the “Tray complete” and none of the instruments are missing or extra.

