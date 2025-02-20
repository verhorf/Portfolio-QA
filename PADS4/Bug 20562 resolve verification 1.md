## Test Case: Verify Fix for Rule Based on Day of Datetime in PADS4 Designer

### **Test ID:** TC_20562

### **Title:** Verify that rule based on day of datetime works correctly in PADS4 Designer

### **Preconditions:**
- Installed version: PADS4 Designer 4.12.7725
- System running Windows 11 Enterprise

### **Test Steps:**

1. Open **PADS4 Designer**.
2. Navigate to **System > About** and confirm that the installed version is **4.12.7725**.
3. Click on **File > New Presentation**.
4. In the new window, keep all parameters at default and click **Create**.
5. Add a text element:
   - On the left panel, click the **Text** tool.
   - Draw a text area at position **Start Position (0,0)** and **End Position (100,100)**.
6. Open text element properties:
   - Double-click the text element **or** right-click and select **Properties**.
7. Modify text properties:
   - Add test text: **"Test rule based on day of datetime"**.
   - Set font size to **12** to ensure visibility.
8. Navigate to the **Rules** tab within the properties panel.
9. Add a new rule:
   - **Rule:** `If [CurrentDateTime] < {Enter Date Time} Then (hide element).`
   - Set `{Enter Date Time}` to a **future** timestamp in the format **HH:MM DD/MM/YYYY**.
10. Save the changes by clicking **Save**.
11. Click **Preview** on the toolbar **or** press `F10` to start the presentation preview.

### **Expected Result:**
- The text element should **not be visible** in the preview if the current datetime is less than the specified `{Enter Date Time}`.

### **Actual Result:**
- The text does not appear in the presentation as expected.

### **Status:** ✅ Pass / ❌ Fail (to be marked after execution)
