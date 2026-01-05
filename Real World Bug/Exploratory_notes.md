# Exploratory Testing Notes

## Context
While browsing CS2 items on Tradeit.gg, I was looking for items with the best quality based on float value.
Float value is commonly used by users to evaluate item condition (Good or Bad).

## How the issue was discovered
During normal browsing, I attempted to sort items by lowest float value to quickly compare item quality.
At this point, I noticed the sorting order did not appear correct.

## Exploration Performed
- Applied sorting by float value (ascending)
- Observed the displayed float values
- Disabled all active filters to eliminate filter related factors
- Re-applied float sorting
- Compared the behavior with sorting by price

## Findings
- Float values were displayed not in order (e.g. 0.9 → 0.4 → 0.8 → 0.7)
- The behavior was reproducible after refreshing and repeating the steps
- Sorting by price worked as expected under the same conditions

## Patterns
- Issue only occurs when sorting by float value
- Consistently reproducible
- Not affected by filters

## User Impact
- Users may struggle to identify item quality
- Increased effort to find desired items
- Reduced trust in sorting functionality

## Conclusion
Based on repeated exploration and comparison with other sorting options, this appears to be a defect isolated to float value sorting behavior.
