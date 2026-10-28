
# Accessibility Audit Report

## 1. Project Information

- **Project Name:** My Site
- **Page Audited:** index.html
- **Date:** 28 October 2026

## 2. Tools Used

1. Google Chrome DevTools Lighthouse
2. WAVE Web Accessibility Evaluation Tool

## 3. Issues Found and How I Fixed Them

### Issue 1: Images Missing Alternative Text

**Problem:**  
Images without alternative text may be inaccessible to users who rely on screen readers.

**Fix:**  
Added descriptive alt attributes to meaningful images. Decorative images use empty alt attributes.

**Example:**
```html
<img src="logo.png" alt="My Site logo">
```

### Issue 2: Incorrect Heading Hierarchy

**Problem:**  
Headings that do not follow a logical structure can make navigation difficult for screen reader users.

**Fix:**  
Organized headings using h1 for the main page heading, h2 for major sections, and h3 for subsections where appropriate.

**Example:**
```html
<h1>Welcome to My Site</h1>
<h2>About Us</h2>
<h3>Our Mission</h3>
```

### Issue 3: Non-Descriptive Link Text

**Problem:**  
Generic links such as "Click here" do not clearly explain their purpose.

**Fix:**  
Used descriptive link text that explains the destination.

**Example:**
```html
<a href="contact.html">Contact our team</a>
```

### Issue 4: Missing Language Attribute

**Problem:**  
The page language was not specified, which may affect screen reader pronunciation.

**Fix:**  
Added the lang attribute to the html element.

**Example:**
```html
<html lang="en">
```

### Issue 5: Form Labels

**Problem:**  
Form inputs without associated labels can be difficult to understand when using assistive technologies.

**Fix:**  
Associated each label with its form control using matching for and id attributes.

**Example:**
```html
<label for="email">Email Address</label>
<input type="email" id="email" name="email" required>
```

## 4. Lighthouse Accessibility Audit

**Tool:** Chrome DevTools Lighthouse

**Testing procedure:**
1. Opened index.html in Google Chrome.
2. Opened Chrome DevTools.
3. Selected the Lighthouse panel.
4. Selected the Accessibility category.
5. Ran the accessibility audit.
6. Reviewed the findings and corrected applicable issues.
7. Ran the audit again.

**Results:**
- Initial accessibility score: Not yet recorded.
- Final accessibility score: Not yet recorded.
- Remaining issues: Not yet recorded.

## 5. WAVE Accessibility Audit

**Tool:** WAVE Web Accessibility Evaluation Tool  
**Website:** https://wave.webaim.org/

**Testing procedure:**
1. Opened the WAVE website.
2. Entered the URL of the page being tested, if publicly accessible.
3. Reviewed the errors, alerts, and accessibility features.
4. Corrected applicable issues.
5. Re-tested the page.

**Results:**
- Initial errors: Not yet recorded.
- Final errors: Not yet recorded.
- Remaining alerts: Not yet recorded.

## 6. Conclusion

The accessibility review focused on alternative text for images, heading hierarchy, descriptive links, document language, and form labels.

The HTML was updated to address these accessibility requirements. Lighthouse and WAVE testing must be completed to verify the changes and record the final results.

Manual keyboard navigation and screen reader testing are also recommended because automated tools cannot detect every accessibility problem.

## 7. References

- Chrome Lighthouse: https://developer.chrome.com/docs/lighthouse/
- WAVE Accessibility Tool: https://wave.webaim.org/
- Web Accessibility Initiative (WAI): https://www.w3.org/WAI/
