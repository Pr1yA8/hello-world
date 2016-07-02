# hello-world
Just other repository
<!DOCTYPE html>
<html>
  <head>
    <style>
      html,
      body {
        font-family: Arial, sans-serif;
        height: 100%;
        margin: 0;
        padding: 0;
      }
      #map {
        height: 100%;
      }
    </style>
  </head>
  <body>
    <div id="map"></div>
    <script>
      var map;
      function initMap() {
        // Constructor creates a new map - only center and zoom are required.
        map = new google.maps.Map(document.getElementById('map'), {
          center: {lat: 40.7413549, lng: -73.9980244},
          zoom: 13
        });
        var tribeca = {lat: 40.719526, lng: -74.0089934};
        var marker = new google.maps.Marker({
          position: tribeca,
          map: map,
          title: 'First Marker!'
        });
      }
    </script>

    <script async defer
        src="https://maps.googleapis.com/maps/api/js?key=MYAPIKEY&v=3&callback=initMap">
    </script>

  </body>
</html>
