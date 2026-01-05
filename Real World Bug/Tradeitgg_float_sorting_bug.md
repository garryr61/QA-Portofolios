# Bug Report: Float Sorting Does Not Work Correctly

## Summary
Sorting items by float value does not work as expected.  
When users apply "Float: Lowest to Highest", "Highest to Lowest" the items appear in random order instead of ascending or descending float values in order.

---

## Environment
- Website: https://tradeit.gg
- Device: Desktop
- OS: Windows 11
- Browser: Google Chrome
- Browser Version: Latest
- Date Found: 5 January 2026

---

## Preconditions
- User opens tradeit.gg
- User is on item listing / marketplace page
- All filters are turned OFF except Float sorting

---

## Steps to Reproduce
1. Open https://tradeit.gg
2. Navigate to the item marketplace page
3. Ensure all filters are disabled
4. Select sorting option: **Float (Lowest to Highest)** / **Float (Highest to Lowest)**
5. Observe the order of float values displayed

---

## Expected Result
Items should be sorted in ascending or descending order based on float value, for example:
0.03 → 0.12 → 0.45 → 0.78 → 0.90  **(Lowest to Highest)**
0.90 → 0.78 → 0.45 → 0.12 → 0.03 **(Highest to Lowest)**

---

## Actual Result
Items are displayed in an inconsistent and random order, for example:
0.90 → 0.42 → 0.78 → 0.65 → 0.30

---

## Frequency
Always (100%)

---

## Severity
Medium

---

## Priority
Low (P2)

---

## Impact
Users who rely on float value to evaluate item quality may:
- Be unable to accurately compare items based on float value
- Spend more time manually checking each item
- Potentially abandon purchase decisions
- Experience degraded user experience and reduced trust in sorting functionality

---

## Additional Notes
- Price sorting works correctly
- The issue only occurs when sorting by float value
- Issue persists even when all other filters are disabled

---

## Evidence
- Screenshot will be attached in `/Evidence` folder
