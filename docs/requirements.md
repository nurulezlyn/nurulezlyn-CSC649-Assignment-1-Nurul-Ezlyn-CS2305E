# Requirements

## Functional requirements

| ID | Requirement |
|---|---|
| FR1 | The system shall allow the user to submit a tray image in JPG or PNG format. |
| FR2 | The system shall reject any uploaded file that is not a readable JPG or PNG image and display an error message. |
| FR3 | The system shall detect all instruments in the submitted image that belong to any of the instrument classes being supported. |
| FR4 | The system shall assign a class label to each detection. |
| FR5 | The system shall allocate each detection a confidence score. |
| FR6 | The system shall accept only if its confidence score exceeds or equal to the confidence threshold (default is 0.50). |
| FR7 | The system shall count the accepted detections for each supported class separately. |
| FR8 | The system shall let the user choose a predefined tray checklist before doing the reconciliation. |
| FR9 | The system  shall compare the detected count of each class with the count on the presented selected checklist. |
| FR10 | The system shall show each class with fewer than the expected count. |
| FR11 | The system shall show each class with more than the expected count. |
| FR12 | The system shall show the uploaded image with bounding boxes around the detected instruments. |
| FR13 | The system shall display a “Tray complete” status when the detected count corresponds with the checklist count for each class. |

## Non-functional requirements

| ID | Type | Measurable requirement |
|---|---|---|
| NFR1 | Performance | The system should be able to identify and reconcile results in less than 10 seconds for any image on the testing machine. |
| NFR2 | Accuracy | The detection model shall achieve a score at least 0.80 mAP@0.5 on the test dataset. |
| NFR3 | Usability | A first time user shall complete the tray checking process in under 3 minutes. |
| NFR4 | Security | Uploaded images will not be kept after the result is displayed unless the user decides to store them. |
| NFR5 | Reliability | The system should display a clear error message for 100% of invalid files (wrong format or corrupt image). |
