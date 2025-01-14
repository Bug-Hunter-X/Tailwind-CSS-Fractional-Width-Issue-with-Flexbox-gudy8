# Tailwind CSS Fractional Width Issue with Flexbox

This repository demonstrates a common issue encountered when using Tailwind CSS's fractional width classes (`w-1/2`, `w-1/3`, etc.) within a flexbox container.  The issue arises when the fractional width classes don't behave as expected, leading to unexpected layout issues.

**Problem:** The `w-1/2` classes applied to the divs within the flex container don't correctly divide the container's width into two equal halves.  This occurs because the flexbox layout model has its own mechanisms for sizing its children.

**Solution:** This issue can be resolved by either removing the fractional width classes or using flex-grow to control the width of the children within the flex container.

See `bug.html` for the erroneous implementation and `bugSolution.html` for the solution.