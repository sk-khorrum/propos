# propos
Propos thim
<div id="cartoon">

  <img id="boy" src="boy.png" alt="Boy Cartoon">

  <img id="flower" src="flower.png" alt="Flower">

  <button onclick="animateCartoon()">Propose</button>

</div>

#cartoon {

  position: relative;

  width: 300px;

  height: 300px;

}

#boy {

  position: absolute;

  top: 0;

  left: 0;

  width: 100%;

  height: 100%;

}

#flower {

  position: absolute;

  top: 80px;

  left: 150px;

  width: 50px;

  height: 50px;

  opacity: 0;

}

#cartoon {

  position: relative;

  width: 300px;

  height: 300px;

}

#boy {

  position: absolute;

  top: 0;

  left: 0;

  width: 100%;

  height: 100%;

}

#flower {

  position: absolute;

  top: 80px;

  left: 150px;

  width: 50px;

  height: 50px;

  opacity: 0;

}

function animateCartoon() {

  var flower = document.getElementById("flower");

  flower.style.opacity = "1";

  var tween = new TimelineLite();

  tween.to(flower, 1, {left: "200px", top: "150px"})

       .to(flower, 0.5, {rotation: 360})

       .to(flower, 1, {left: "150px", top: "80px"})

       .to(flower, 1, {opacity: 0});

}

