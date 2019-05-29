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
