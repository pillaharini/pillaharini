<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Gallery</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.1.0/magnific-popup.min.css">
    <link rel="stylesheet" href="Gallary.css">
</head>
<body>
    <div class="inp">
        <p class="para">SelfCare..SelfLove..</p>
    </div>
    <div class="gallery">
        <ul class="controls">
            <li class="buttons active" data-filter="All">All</li>
            <li class="buttons" data-filter="Cleanser">Cleanser</li>
            <li class="buttons" data-filter="Serum">Serum</li>
            <li class="buttons" data-filter="Moisturizer">Moisturizer</li>
            <li class="buttons" data-filter="EyeCream">EyeCream</li>
            <li class="buttons" data-filter="Sunscreen">Sunscreen</li>
            <li class="buttons" data-filter="Masks">Masks</li>
        </ul> 
        <div class="image-container">
            <a href="D:\cleanser1.webp" class="image Cleanser">
                <img src="D:\cleanser1.webp" alt="">
            </a>
            <a href="D:\cleanser2.webp" class="image Cleanser">
                <img src="D:\cleanser2.webp" alt="">
            </a>
            <a href="D:\cleanser3.jpeg" class="image Cleanser">
                <img src="D:\cleanser3.jpeg" alt="">
            </a>
            <a href="D:\cleanser4.webp" class="image Cleanser">
                <img src="D:\cleanser4.webp" alt="">
            </a>
            <a href="D:\cleanser5.avif" class="image Cleanser">
                <img src="D:\cleanser5.avif" alt="">
            </a>
            <a href="D:\serum1.jpg" class="image Serum">
                <img src="D:\serum1.jpg" alt="">
            </a>
            <a href="D:\serum2.jpg" class="image Serum">
                <img src="D:\serum2.jpg" alt="">
            </a>
            <a href="D:\serum3.webp" class="image Serum">
                <img src="D:\serum3.webp" alt="">
            </a>
            <a href="D:\serum4.webp" class="image Serum">
                <img src="D:\serum4.webp" alt="">
            </a>
            <a href="D:\serum5.jpg" class="image Serum">
                <img src="D:\serum5.jpg" alt="">
            </a>
            <a href="D:\moisturizer1.webp" class="image Moisturizer">
                <img src="D:\moisturizer1.webp" alt="">
            </a>
            <a href="D:\moisturizer2.webp" class="image Moisturizer">
                <img src="D:\moisturizer2.webp" alt="">
            </a>
            <a href="D:\moisturizer3.jpeg" class="image Moisturizer">
                <img src="D:\moisturizer3.jpeg" alt="">
            </a>
            <a href="D:\moisturizer4.webp" class="image Moisturizer">
                <img src="D:\moisturizer4.webp" alt="">
            </a>
            <a href="D:\moisturizer5.webp" class="image Moisturizer">
                <img src="D:\moisturizer5.webp" alt="">
            </a>
            <a href="D:\eyecream1.avif" class="image EyeCream">
                <img src="D:\eyecream1.avif" alt="">
            </a>
            <a href="D:\eyecream2.webp" class="image EyeCream">
                <img src="D:\eyecream2.webp" alt="">
            </a>
            <a href="D:\eyecream3.avif" class="image EyeCream">
                <img src="D:\eyecream3.avif" alt="">
            </a>
            <a href="D:\eyecream4.jpg" class="image EyeCream">
                <img src="D:\eyecream4.jpg" alt="">
            </a>
            <a href="D:\eyecream5.webp" class="image EyeCream">
                <img src="D:\eyecream5.webp" alt="">
            </a>
            <a href="D:\ss1.jpeg" class="image Sunscreen">
                <img src="D:\ss1.jpeg" alt="">
            </a>
            <a href="D:\ss2.webp" class="image Sunscreen">
                <img src="D:\ss2.webp" alt="">
            </a>
            <a href="D:\ss3.webp" class="image Sunscreen">
                <img src="D:\ss3.webp" alt="">
            </a>
            <a href="D:\ss4.webp" class="image Sunscreen">
                <img src="D:\ss4.webp" alt="">
            </a>
            <a href="D:\ss5.webp" class="image Sunscreen">
                <img src="D:\ss5.webp" alt="">
            </a>
            <a href="D:\mask1.avif" class="image Masks">
                <img src="D:\mask1.avif" alt="">
            </a>
            <a href="D:\mask2.webp" class="image Masks">
                <img src="D:\mask2.webp" alt="">
            </a>
            <a href="D:\mask3.jpg" class="image Masks">
                <img src="D:\mask3.jpg" alt="">
            </a>
            <a href="D:\mask4.jpg" class="image Masks">
                <img src="D:\mask4.jpg" alt="">
            </a>
            <a href="D:\mask5.webp" class="image Masks">
                <img src="D:\mask5.webp" alt="">
            </a>
        </div>
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.1.0/jquery.magnific-popup.min.js"></script>
    <script>
        $(document).ready(function(){
            $('.buttons').click(function(){
                $(this).addClass('active').siblings().removeClass('active');
                var filter = $(this).attr('data-filter');
                if (filter == 'All') {
                    $('.image').show(400); // Show all images if 'All' is selected
                } else {
                    $('.image').hide(200).filter('.' + filter).show(400); // Show only selected filter images
                }
            });
            $('.gallery').magnificPopup({
                delegate:'a',
                type:'image',
                gallery:{
                    enabled:true
                }
            })
        });
    </script>
</body>
</html>

<!---
pillaharini/pillaharini is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
