# Browser Inconsistency in CSS
This repository demonstrates a common CSS bug: inconsistent rendering across different browsers due to the use of non-standard or poorly supported CSS properties.  The `bug.css` file showcases the issue, while `bugSolution.css` provides the corrected code.

## Problem
The original CSS uses a vendor-specific prefix (`-webkit-`) without including the standard property.  This results in the style only applying to WebKit-based browsers.  Other browsers will not render the style correctly, leading to an inconsistent user experience.

## Solution
The solution involves using the standard CSS property (`box-shadow`) alongside the vendor-specific prefix as a fallback. This ensures broad compatibility across modern and older browsers.