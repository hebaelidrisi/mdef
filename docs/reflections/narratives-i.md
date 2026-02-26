## Pictorial

<style>
    .slideshow-container {
    max-width: 100%; /* Now matches the width of your other page images */
    position: relative;
    margin: 40px auto;
    border-radius: 20px;
    overflow: hidden;
    box-shadow: 0 10px 30px rgba(0,0,0,0.15);
}
    .mySlides { display: none; text-align: center; }
    .mySlides img { width: 100%; height: auto; display: block; border-radius: 20px; }
    .numbertext { color: #333; font-size: 14px; padding: 12px 0; text-align: center; width: 100%; }
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
        border-radius: 50%;
        background-color: rgba(0,0,0,0.3);
        user-select: none;
        text-decoration: none !important;
        z-index: 100;
    }
    .next { right: 15px; }
    .prev { left: 15px; }
    .prev:hover, .next:hover { background-color: rgba(0,0,0,0.8); }
</style>

<div class="slideshow-container" markdown="1">

<div class="mySlides">
<img src="../../images/pictorial-draft-1.jpg" alt="Cover">
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

        // CUSTOM COUNTER LOGIC
        let pageDisplay = "";
        if (slideIndex === 1) {
            pageDisplay = "1";
        } else if (slideIndex === 2) {
            pageDisplay = "2-3";
        } else if (slideIndex === 3) {
            pageDisplay = "4-5";
        } else if (slideIndex === 4) {
            pageDisplay = "6-7"; // Added in case you add another spread later
        }

        if(counter) { 
            counter.innerHTML = pageDisplay; 
        }
    }
</script>

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


## Peer Interpretation Snapshot (Ayal)

![](../images/pictorial-snapshot.png)

### Abstract & References

#### Abstract

I envision my pictorial resembling a museum catalogue that represents the relationship between objects, earth material and human memory. The pictorial would treat the material objects as condensed archives of time and narratives. The content would be centered around the visual typology of the selected objects, with classification labels and associated narratives to build the archive. I want to use the catalogue style to define the structure while creating a simple but legible pictorial. Objects will be visually divided into different sections of physical appearance, origins, associated human memories, and abstracted visual study. The reason I want to use this structuring style and organization is to allow the material’s complexity to shape the visual realm and create a flexible archive of contents. 

#### References

![](../images/pictorial_references.jpg)