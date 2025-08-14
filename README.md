<!DOCTYPE html>
<html>
<head>
  <title>Карта переработки мусора в Казахстане</title>
  <style>
    /* Карта занимает весь экран */
    #map {
      height: 100vh;
      width: 100%;
    }
  </style>
  <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap" async defer></script>
  <script>
    function initMap() {
      // Центр на Казахстане
      var kazakhstanCenter = { lat: 48.0196, lng: 66.9237 };

      // Создаём карту
      var map = new google.maps.Map(document.getElementById('map'), {
        zoom: 5,
        center: kazakhstanCenter
      });

      // Пример координат пунктов переработки
      var recyclingPoints = [
        { lat: 43.2389, lng: 76.8897, name: 'Пункт переработки Алматы' },
        { lat: 51.1694, lng: 71.4491, name: 'Пункт переработки Астана' },
        { lat: 50.2839, lng: 57.1660, name: 'Пункт переработки Актобе' }
      ];

      // Добавляем маркеры
      recyclingPoints.forEach(function(point) {
        new google.maps.Marker({
          position: { lat: point.lat, lng: point.lng },
          map: map,
          title: point.name,
          icon: {
            url: "http://maps.google.com/mapfiles/ms/icons/green-dot.png"
          }
        });
      });
    }
  </script>
</head>
<body>
  <div id="map"></div>
</body>
</html>
