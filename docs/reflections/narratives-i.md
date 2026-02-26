## Pictorial

<style>
    /* Container for the flipbook */
    .slideshow-container {
        max-width: 80%; /* Adjusted for double-page spreads */
        position: relative;
        margin: 40px auto;
        border-radius: 20px; /* Curved edges as requested */
        overflow: hidden;
        box-shadow: 0 10px 30px rgba(0,0,0,0.15);
        background-color: #f9f9f9;
    }

    /* Hide slides by default */
    .mySlides {
        display: none;
        text-align: center;
    }

    /* Style for the images */
    .mySlides img {
        width: 100%;
        height: auto;
        display: block;
        border-radius: 20px; /* Ensures images follow the curve */
    }

    /* Counter text (1/4, etc.) */
    .numbertext {
        color: #333;
        font-size: 14px;
        padding: 12px 0;
        text-align: center;
        width: 100%;
    }

    /* Navigation Arrows */
    .prev, .next {
        cursor: pointer;
        position: absolute;
        top: 50%;
        width: auto;
        padding: 16px;
        margin-top: -22px;
        color: white;
        font-weight: bold;
        font-size: 18px;
        transition: 0.3s ease;
        border-radius: 50%; /* Circular buttons */
        background-color: rgba(0,0,0,0.3);
        user-select: none;
        text-decoration: none !important;
    }

    .next { right: 15px; }
    .prev { left: 15px; }

    .prev:hover, .next:hover {
        background-color: rgba(0,0,0,0.8);
    }
</style>

<div class="slideshow-container">
    <div class="mySlides">
        <img src="../../images/pictorial-draft-1.jpg" alt="Cover Page">
    </div>

    <div class="mySlides">
        <img src="../../images/pictorial-draft-2.jpg" alt="Spread 1">
    </div>

    <div class="mySlides">
        <img src="../../images/pictorial-draft-3.jpg" alt="Spread 2">
    </div>

    <div class="mySlides">
        <img src="../../images/pictorial-draft-4.jpg" alt="Spread 3">
    </div>
    
    ...
</div>

    <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
    <a class="next" onclick="plusSlides(1)">&#10095;</a>
</div>

<div id="counter" class="numbertext">1 / 4</div>

<script>
    let slideIndex = 1;
    showSlides(slideIndex);

    function plusSlides(n) {
        showSlides(slideIndex += n);
    }

    function showSlides(n) {
        let i;
        let slides = document.getElementsByClassName("mySlides");
        let counter = document.getElementById("counter");
        
        if (n > slides.length) {slideIndex = 1}    
        if (n < 1) {slideIndex = slides.length}
        
        for (i = 0; i < slides.length; i++) {
            slides[i].style.display = "none";  
        }
        
        slides[slideIndex-1].style.display = "block";  
        counter.innerHTML = slideIndex + " / " + slides.length;
    }
</script>

![](../images/pictorial-draft-1.jpg)
![](../images/pictorial-draft-2.jpg)
![](../images/pictorial-draft-3.jpg)
![](../images/pictorial-draft-4.jpg)

## Peer Interpretation Snapshot (Ayal)

![](../images/pictorial-snapshot.png)

### Abstract & References

#### Abstract

I envision my pictorial resembling a museum catalogue that represents the relationship between objects, earth material and human memory. The pictorial would treat the material objects as condensed archives of time and narratives. The content would be centered around the visual typology of the selected objects, with classification labels and associated narratives to build the archive. I want to use the catalogue style to define the structure while creating a simple but legible pictorial. Objects will be visually divided into different sections of physical appearance, origins, associated human memories, and abstracted visual study. The reason I want to use this structuring style and organization is to allow the material’s complexity to shape the visual realm and create a flexible archive of contents. 

#### References

![](../images/pictorial_references.jpg)