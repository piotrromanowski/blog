---
title: "Photography"
date: 2019-06-18T18:56:07-04:00
draft: false
---

<h1>Denver</h1>
<div class="grid-container">
    <img id="a" class="a" src="https://piotrromanowski.github.io/images/denver-a.jpg">
    <img id="b" class="b" src="https://piotrromanowski.github.io/images/denver-b.jpg">
    <img id="c" class="c" src="https://piotrromanowski.github.io/images/denver-c.jpg">
    <img id="d" class="d" src="https://piotrromanowski.github.io/images/denver-d.jpg">
    <img id="e" class="e" src="https://piotrromanowski.github.io/images/denver-e.jpg">
    <img id="f" class="f" src="https://piotrromanowski.github.io/images/denver-f.jpg">
</div>
<div class="grid-container">
<div>


<!-- The Modal -->
<div id="myModal" class="modal">
  <img class="modal-content" id="img01">
</div>


<script>
  var modal = document.getElementById('myModal');

  // Get the image and insert it inside the modal - use its "alt" text as a caption
  images = ['a', 'b', 'c', 'd', 'e', 'f'];

  for (image of images) {
    var img = document.getElementById(image);
    var modalImg = document.getElementById("img01");
    //var captionText = document.getElementById("caption");
    img.onclick = function(){
        modal.style.display = "block";
        modalImg.src = this.src;
        modalImg.alt = this.alt;
        //captionText.innerHTML = this.alt;
    }
  }


  // When the user clicks on <span> (x), close the modal
  modal.onclick = function() {
      img01.className += " out";
      setTimeout(function() {
        modal.style.display = "none";
        img01.className = "modal-content";
      }, 400);
      
  }
</script>
