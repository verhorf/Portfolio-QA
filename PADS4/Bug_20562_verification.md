# Test Case: Verify Rule-Based Visibility of Text Element in PADS4 Designer

## Test Case 1: Element Should Be Hidden Before Specified DateTime

### Steps:
1. Open PADS4 Designer.
2. Navigate to **System > About** to ensure the software is updated to the latest version.
3. Click **File > New Presentation**.
4. In the new window, keep all parameters at default and click **Create**.
5. Add a **Text** element by clicking the **Text** button on the toolbar.
6. Draw the text element in the position **Start Position(0,0), End Position(100,100)**.
7. Open the properties of the Text element (double-click it or right-click and select **Properties**).
8. Add sample text **"Test rule based on day of datetime"** and set the font size to **12** for visibility.
9. Navigate to the **Rules** tab within the properties.
10. Add a new rule: **If [CurrentDateTime] < {Enter Date Time} Then (hide element).**
	- `{Enter Date Time}` should be set in the future so that the element remains hidden until that time.
11. Save the changes by clicking **Save**.
12. Start **Preview** mode by clicking the **Preview** button on the top toolbar or pressing **F10**.

### Expected Result:
- The text element should not be visible in the presentation preview.

### Actual Result:
- The text does not appear in the presentation.

---

## Test Case 2: Element Should Become Visible After Specified DateTime

### Steps:
1. Open PADS4 Designer.
2. Navigate to **System > About** to ensure the software is updated to the latest version.
3. Click **File > New Presentation**.
4. In the new window, keep all parameters at default and click **Create**.
5. Add a **Text** element by clicking the **Text** button on the toolbar.
6. Draw the text element in the position **Start Position(0,0), End Position(100,100)**.
7. Open the properties of the Text element (double-click it or right-click and select **Properties**) and enable the **Hidden** checkbox.
8. Add sample text **"Test rule based on day of datetime"** and set the font size to **12** for visibility.
9. Navigate to the **Rules** tab within the properties.
10. Add a new rule: **If [CurrentDateTime] > {Enter Date Time} Then (show element).**
	- `{Enter Date Time}` should be set in the past so that the element becomes visible when the rule is applied.
11. Save the changes by clicking **Save**.
12. Start **Preview** mode by clicking the **Preview** button on the top toolbar or pressing **F10**.

### Expected Result:
- The text element should become visible in the presentation preview.

### Actual Result:
- The text appears in the presentation as expected.
