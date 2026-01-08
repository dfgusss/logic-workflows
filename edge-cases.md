# Edge Case Scenarios

## Case 1: Empty CSV File
- File type: CSV
- File size: > 5MB
Expected:
- Reject file with reason: "File contains no data"

## Case 2: CSV with Invalid Encoding
Expected:
- Reject file with reason: "Invalid file encoding"

## Case 3: CSV with Missing Required Columns
Expected:
- Reject file with detailed column error
