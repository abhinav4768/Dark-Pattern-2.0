# Dark-Pattern-2.0
This Repository contains files of HTML, CSS, JS which you can access. This is the project of Browser Extension to find dark pattern on websites.
# JSON File
{
    "name":"Dark Pattern 2.0",
    "version": "0.0.1",
    "manifest_version": 2,
    "browser_action": {
        "default_popup":"popup.html",
        "default_icon":"logo.png"
    },
    "icons":{
        "128":"logo.png",
    },
    "permisssions":["activeTab"]
    
}

# HTML File 
<!DOCTYPE html>
<html lang="en">
<head>
      <meta charset="UTF-8">
      <meta http-equiv="X-UA-Compatible" content="IE=edge">
      <meta name="viewport" content="width=device-width, initial-s"
      <title>Dark Pattern 2.0</title>
</head>
<body>
    <p>Dark Patterns will be found here</p>
</body>
</html>

# CSS File
body {
width:300px;
height:300px;
background-color: aliceblue;
display: flex;
justify-content: center;
}

p {
    display: inner-flex;
    margin: auto 10px;
    font-size: 22px;
    color: blue;
    border-radius: 6px;
    border: 1px solid lightblue;
    padding: 10px;

}

# JAVA Script File

fetch('chrome.webRequest')
.then(data=>data.json())
.then(DarkPatternData => {
    const DarkPatternText = DarkPatternData.attachments[0].text;
    const DarkPatternElement = document.getElementById('DarkPatternElement');
    DarkPatternElement.innerHTML = DarkPatternText;
})

# LOGO.PNG
