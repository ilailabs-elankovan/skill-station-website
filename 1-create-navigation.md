## 1 Create a Navigation Bar

• Create a navigation bar with three buttons, that can help the user to naviagate to the three sections correspondingly 

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .sections {
      background-color: #e4e1e1;
    }

    .menu {
      background-color: rgb(127, 148, 148);
      padding: 20px;
      text-align: right;
    }

    .button-container {
      background-color: rgb(31, 48, 48);
      width: 50%;
      text-align: right;
    }

    .section-one {
      background-color: #f0f0f0;
      /* Replace with your desired color */
      padding: 20px;
      /* Optional: Add some padding for better visibility */
      height: 480px;
      margin-bottom: 10px;
    }

    .section-two {
      background-color: #eccece;
      /* Replace with your desired color */
      padding: 20px;
      /* Optional: Add some padding for better visibility */
      height: 480px;
      margin-bottom: 10px;
    }

    .section-three {
      background-color: #d1b8b8;
      /* Replace with your desired color */
      padding: 20px;
      /* Optional: Add some padding for better visibility */
      height: 480px;
      margin-bottom: 10px;
    }

    .section {
      height: 480px;
    }
  </style>
  <title>Skill Station</title>
</head>

<body>

  <div class="menu">
    <div class="button-container">
      <button id="section-one-btn" onclick="scrollToSection('section-1')">Section One</button>
      <button id="section-two-btn" onclick="scrollToSection('section-2')">Section Two</button>
      <button id="section-three-btn" onclick="scrollToSection('section-3')">Section Three</href></button>
    </div>
  </div>

  <div class="sections">
    <div class="section">
      <p1>Section One</p1>
    </div>

    <div class="section" id="section-2">
      <p1>Section Two</p1>
    </div>

    <div class="section" id="section-3">
      <p1>Section Three</p1>
    </div>
  </div>

  <script>
    function myPrint() {
      console.log("myPrint executed")

    }

    function scrollToSection(sectionId) {
      const section = document.getElementById(sectionId);

      if (section) {
        section.scrollIntoView({ behavior: 'smooth' });
      } else {
        console.error(`Section with id '${sectionId}' not found.`);
      }
    }
  </script>
</body>

</html>
<!DOCTYPE html>
<html lang="en">

<head>

</head>
```
