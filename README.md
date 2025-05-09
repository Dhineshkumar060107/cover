# Ex.06 Book Front Cover Page Design
## Date:27/04/2025

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Book Cover with Author Photo</title>

  <style>
    /* Basic reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      height: 100vh;
      background: linear-gradient(135deg, #dbe6f6, #c5796d);
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: Georgia, serif;
    }

    .cover {
      width: 400px;
      height: 600px;
      background: url('https://images.unsplash.com/photo-1498050108023-c5249f4df085?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=60') center/cover no-repeat;
      border-radius: 12px;
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
      position: relative;
      overflow: hidden;
      padding: 20px;
      display: flex;
      flex-direction: column;
    }

    /* Overlay for readability */
    .cover::before {
      content: "";
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background-color: rgba(255, 255, 255, 0.85);
      z-index: 0;
    }

    .cover-content {
      position: relative;
      z-index: 1;
      display: flex;
      flex-direction: column;
      height: 100%;
      text-align: center;
    }

    .cover-content img.cover-image {
      width: 100%;
      height: 250px;
      object-fit: cover;
      border-radius: 8px;
      margin-bottom: 20px;
    }

    .title {
      font-size: 28px;
      font-weight: bold;
      color: #333;
      margin-bottom: 10px;
    }

    .subtitle {
      font-size: 18px;
      color: #555;
      margin-bottom: 20px;
    }

    /* Author photo styling */
    .author-photo {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      object-fit: cover;
      margin: 0 auto 15px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }

    .author {
      font-size: 20px;
      font-weight: 600;
      color: #222;
      margin-bottom: 20px;
    }

    .footer {
      font-size: 14px;
      color: #777;
    }
  </style>
</head>

<body>

  <div class="cover">
    <div class="cover-content">
      <img 
        src="https://images.unsplash.com/photo-1496181133206-80ce9b88a853?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=60" 
        alt="Cover Image"
        class="cover-image"
      >

      <div class="title">The Art of Possibility</div>
      <div class="subtitle">Unlocking Creativity and Vision</div>

      
      <img 
        src="dhinesh/bookapp/static/fotor-20250427183212.jpg"
        alt="Author photo" 
        class="author-photo"
      >

      <div class="author">By Dhineshkumar.L</div>
      <div class="footer">Published 2025</div>
    </div>
  </div>

</body>
</html>
```


## OUTPUT:


![alt text](<Screenshot 2025-04-27 185252.png>)
![alt text](<Screenshot 2025-04-27 185738.png>)


## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
