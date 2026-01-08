# File Validation Flow

## Objective
Validate incoming files before processing.

## Logic Flow

IF file type is NOT CSV  
→ Reject file with reason: "Unsupported file type"

IF file type is CSV  
AND file size < 5MB  
→ Skip cleaning process

IF file type is CSV  
AND file size >= 5MB  
→ Run data cleaning process

## Notes
- File size threshold is configurable
- Rejected files should return clear error messages
