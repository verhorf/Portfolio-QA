# Test Case: Verify successful room booking

## Test Case ID: 00002

### Description:
Check that the booking panel can be used to successfully make a booking on a new version.

### Precondition:
- The "Meeting Room Booking Panel" device is required
- Current status on the panel should be "Available"

### Device
Device type: Panel
OS type: Android
OS Version: 11
Booking panel software version: 0.7929

### Steps:
1. Use the "Meeting Room Booking Panel" device.
2. Press the "Quick Booking" button.
3. Use the navigation buttons (e.g., "+" or "-") to select the "15 minutes" booking duration.
4. Click "Ok" button.

### Expected Result:
- The meeting room booking panel has successfully moved to the "Booked".
- The status indicator light turns light green.

### Actual Result:
(To be filled after execution)

### Notes:
- If the meeting room is already booked and it is a test device, you can remove the booking using the "Remove Booking" button to test it.
