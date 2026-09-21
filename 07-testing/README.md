# Cloud Deployment Testing

## Objective

The objective of this test was to verify that the static website deployed to Amazon S3 was accessible and functioning correctly.

## Tests Performed

### Test 1: Website Accessibility

The S3 website endpoint was opened in a web browser.

**Expected result:**
The website should load successfully.

**Result:**
PASS

### Test 2: HTML Page

The `index.html` file was loaded through the website.

**Expected result:**
The website content should be displayed.

**Result:**
PASS

### Test 3: CSS

The `style.css` file was loaded by the website.

**Expected result:**
The website should display the intended styling.

**Result:**
PASS

### Test 4: S3 Objects

The S3 bucket was checked to confirm that the required website files were uploaded.

Files checked:

* `index.html`
* `style.css`

**Result:**
PASS

## Conclusion

The tests confirmed that the static website was successfully deployed to Amazon S3 and that the required website files were accessible.

This demonstrated the basic process of deploying a website to cloud storage and verifying that the deployment works.
