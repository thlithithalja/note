# note

<!DOCTYPE html>
<html table="fr">
    <head>
        <meta charset="utf-8" >

<link href="style/style.css" rel="stylesheet" >
    </head>
    <body>
        <link href="https://fonts.googleapis.com/css?family=Roboto+Slab" rel="stylesheet">

        <div class="series-frame">  
          <h2>Nom Série</h2>
          <p id="first-episode-info"></p>
        </div>
        
        <div class="series-frame">
          <h2>Nom Série</h2>
          <p id="second-episode-info"></p>
        </div>
        
        <div class="series-frame">
          <h2>Nom Série</h2>
          <p id="third-episode-info"></p>
        </div>

        <script src="javascriptl.js"></script>
    </body>
    
</html>


////////////////////////////////


partie JS
///////////////////////////

// Create a class here
// =====================================

class Episode {
  constructor(title, duration, hasBeenWatched) {
    this.title = title;
    this.duration = duration;
    this.hasBeenWatched = hasBeenWatched;
  }
}

let firstEpisode = new Episode('First episode title', 45, true);
let secondEpisode = new Episode('Second episode Title', 45, false);
let thirdEpisode = new Episode('Third episode Title', 60, false);

// =====================================

document.querySelector('#first-episode-info').innerText = `Episode: ${firstEpisode.title}
Duration: ${firstEpisode.duration} min
${firstEpisode.hasBeenWatched ? 'Already watched' : 'Not yet watched'}`;

document.querySelector('#second-episode-info').innerText = `Episode: ${secondEpisode.title}
Duration: ${secondEpisode.duration} min
${secondEpisode.hasBeenWatched ? 'Already watched' : 'Not yet watched'}`;

document.querySelector('#third-episode-info').innerText = `Episode: ${thirdEpisode.title}
Duration: ${thirdEpisode.duration} min
${thirdEpisode.hasBeenWatched ? 'Already watched' : 'Not yet watched'}`;
