## Online regex testers
https://regex101.com/

https://www.regextester.com/

https://regexr.com/

### Regular expression to extract file name from URL in SharePoint

#### 1. In Nintex Workflows

**Pattern:** `^(.*[\\\/])`

**Replacement text:** leave it blank/empty

**Input:** `https://www.sharepoint/abc/test.docx`

**Output:** test.docx

#### 2. In Javascript

**Pattern:** `/^(.*[\\\/])/`

```javascript
function myFunction() {
  var input = "https://www.sharepoint/abc/test.docx"; 
  var output = input.replace(/^(.*[\\\/])/, "");
  console.log(output);
}
```
**Output:** test.docx



### Regular expression to extract file name from URL in SharePoint

#### 1. In Nintex Workflows

**Pattern:** `^.*[\\\/]`

**Replacement text**  : leave it blank/empty

**Input:** `https://www.sharepoint/abc/test.docx`

**Output:** test.docx

#### 2. In Javascript

**Pattern:** `/^.*[\\\/]/`

```javascript
function myFunction() {
  var input = "https://www.sharepoint/abc/test.docx"; 
  var output = input.replace(/^.*[\\\/]/, "");
  console.log(output);
}
```
**Output:** test.docx




### Regular expression to remove file extension form file name

#### 1. In Nintex Workflows

**Pattern:** `\.[^/.]+$`

**Replacement text:** leave it blank/empty

**Input:** `testdoc.aspx`

**Output:** testdoc


#### 2. In Javascript

**Pattern:** `/\.[^/.]+$/g`

```javascript
function myFunction() {
  var input = "testdoc.aspx"; 
  var output = input.replace(/\.[^/.]+$/g, "");
  console.log(output);
}
```
**Output:** testdoc


### Regular expression to accept Integer, decimal & float numbers

#### 1. In Javascript

**Pattern:** `/^[-+]?[0-9]*\.?[0-9]+$/g`

**Valid matches:** 0.7, -0.4, 1, 2, 5.0

**Invalid matches:** ., 0., 7.
