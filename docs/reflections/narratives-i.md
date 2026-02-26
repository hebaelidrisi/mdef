## Pictorial

<p style="text-align:center; max-width:800px; margin:auto;">
Pictorial
</p>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Carousel</title>

 <style>
        /* Container for the entire slideshow */
        .slideshow-container {
            max-width: 800px; /* Max size of the main box */
            position: relative;
            margin: auto;
            border: 1px solid #ddd;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            margin-top: 50px;
        }

        /* Hide the images by default */
        .mySlides {
            display: none;
        }

        /* Style the image itself */
        .mySlides img {
            width: 100%;
            height: auto;
            display: block;
        }

        /* Next & previous buttons (The Arrows) */
        .prev, .next {
            cursor: pointer;
            position: absolute;
            top: 50%;
            width: auto;
            padding: 16px;
            margin-top: -22px;
            color: white;
            font-weight: bold;
            font-size: 20px;
            transition: 0.6s ease;
            border-radius: 0 3px 3px 0;
            user-select: none;
            background-color: rgba(0, 0, 0, 0.5); /* Semi-transparent background */
        }

        /* Position the "next button" to the right */
        .next {
            right: 0;
            border-radius: 3px 0 0 3px;
        }

        /* On hover, add a darker background color */
        .prev:hover, .next:hover {
            background-color: rgba(0, 0, 0, 0.8);
        }

        /* Caption text (optional) */
        .text {
            color: #f2f2f2;
            font-size: 15px;
            padding: 8px 12px;
            position: absolute;
            bottom: 8px;
            width: 100%;
            text-align: center;
        }
    </style>
</head>
<body>

 <div class="slideshow-container">

  <div class="mySlides fade">
            <img src="../images/pictorial-draft-1.jpg" alt="First Image">
            <div class="text">Image 1 of 6</div>
        </div>

  <div class="mySlides fade">
            <img src="../images/pictorial-draft-2.jpg" alt="Second Image">
            <div class="text">Image 2 of 6</div>
        </div>

  <div class="mySlides fade">
            <img src="../images/pictorial-draft-3.jpg" alt="Third Image">
            <div class="text">Image 3 of 6</div>
        </div>

  <div class="mySlides fade">
            <img src="../images/pictorial-draft-4.jpg" alt="Fourth Image">
            <div class="text">Image 4 of 6</div>
        </div>


 <a class="prev" onclick="plusSlides(-1)">&#10094;</a> <a class="next" onclick="plusSlides(1)">&#10095;</a> </div>
    <br>

 <script>
        let slideIndex = 1;
        showSlides(slideIndex);

        // Next/previous controls
        function plusSlides(n) {
            showSlides(slideIndex += n);
        }

        // Main function to show the correct slide
        function showSlides(n) {
            let i;
            let slides = document.getElementsByClassName("mySlides");
            
            // If we are past the last slide, go back to the first
            if (n > slides.length) {
                slideIndex = 1
            }
            
            // If we are before the first slide, go to the last
            if (n < 1) {
                slideIndex = slides.length
            }
            
            // Hide all slides
            for (i = 0; i < slides.length; i++) {
                slides[i].style.display = "none";
            }
            
            // Display the current slide
            slides[slideIndex - 1].style.display = "block";
        }
  </script>

</body>
</html>

![](../images/pictorial-draft-1.jpg)
![](../images/pictorial-draft-2.jpg)
![](../images/pictorial-draft-3.jpg)
![](../images/pictorial-draft-4.jpg)

## Peer Interpretation Snapshot

![](../images/pictorial-snapshot.png)

### Abstract & References

#### Abstract

I envision my pictorial resembling a museum catalogue that represents the relationship between objects, earth material and human memory. The pictorial would treat the material objects as condensed archives of time and narratives. The content would be centered around the visual typology of the selected objects, with classification labels and associated narratives to build the archive. I want to use the catalogue style to define the structure while creating a simple but legible pictorial. Objects will be visually divided into different sections of physical appearance, origins, associated human memories, and abstracted visual study. The reason I want to use this structuring style and organization is to allow the material’s complexity to shape the visual realm and create a flexible archive of contents. 

#### References

![](../images/pictorial_references.jpg)