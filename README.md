# Ex.08 Design of Interactive Image Gallery
## Date:07/05/25

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
</head>
<body>
    <header style="text-align: center; background-color: #333; color: white; padding: 1rem 0;">
        <h1>LONDON</h1>
    </header>

    <div style="white-space: nowrap; overflow-x: auto; padding: 1rem;">
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="Screenshot 2025-03-01 111106.png"style="height:200px">
        </div>
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="Screenshot 2025-03-01 111150.png"style="height:200px">
        </div>
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="Screenshot 2025-03-01 111213.png"style="height:200px">
        </div>
        <div style="display: inline-block;" onclick="openModal(this)">
            <img src="Screenshot 2025-03-01 112359.png"style="height:200px">
        </div>
    </div>

    <div id="modal" style="display: none; position: fixed; z-index: 1; left: 0; top: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.9);">
        <span style="position: absolute; top: 15px; right: 35px; color: white; font-size: 40px; font-weight: bold; cursor: pointer;" onclick="closeModal()">&times;</span>
        <img id="modalImage" style="display: block; margin: 5% auto; max-width: 80%;">
    </div>

    <script>
        function openModal(element) {
            var modal = document.getElementById("modal");
            var modalImg = document.getElementById("modalImage");
            modal.style.display = "block";
            modalImg.src = element.querySelector("img").src;
        }

        function closeModal() {
            document.getElementById("modal").style.display = "none";
        }
    </script>
</body>
</html>


function openModal(element) {
    const modal = document.getElementById("modal");
    const modalImage = document.getElementById("modalImage");
    const caption = document.getElementById("caption");

    modal.style.display = "flex";
    modalImage.src = element.querySelector("img").src;
    caption.textContent = element.querySelector("img").alt;
}

function closeModal() {
    const modal = document.getElementById("modal");
    modal.style.display = "none";
}

```
## OUTPUT:
![Screenshot 2025-05-07 112429](https://github.com/user-attachments/assets/20ea8776-aea5-494c-b408-aa484fc9342c)

![Screenshot 2025-05-07 112448](https://github.com/user-attachments/assets/8e937519-f009-437b-a2dc-c9a95b4de4ee)

![Screenshot 2025-05-07 112523](https://github.com/user-attachments/assets/27d866b4-6587-478c-b851-a1e6207d7b1b)

![Screenshot 2025-05-07 112540](https://github.com/user-attachments/assets/9c317f8c-41cd-4038-8e5a-76fa8080143d)

![Screenshot 2025-05-07 112508](https://github.com/user-attachments/assets/e0ff652c-6173-45e8-bcb9-7bf1a143371e)




## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
