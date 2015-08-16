---
layout: default
title: Contact
permalink: /contact/
---
<div class="row">
  <div class="large-8 columns">

    <h3>Get in Touch!</h3>
    <p>We'd love to hear from you. You can either reach out to us as a whole and one of our awesome team members will get back to you, or if you have a specific question reach out to one of our staff. We love getting email all day <em>all day</em>.</p>

    <div class="section-container tabs" data-section>
      <section class="section">
        <h5 class="title"><a href="#panel1">Contact Our Company</a></h5>
        <div class="content" data-slug="panel1">
          <form action="http://formspree.io/{{ site.email }}">
            <div class="row collapse">
              <div class="large-2 columns">
                <label class="inline">Your Name</label>
              </div>
              <div class="large-10 columns">
                <input type="text" id="yourName" placeholder="Jane Smith">
              </div>
            </div>
            <div class="row collapse">
              <div class="large-2 columns">
                <label class="inline"> Your Email</label>
              </div>
              <div class="large-10 columns">
                <input type="text" id="yourEmail" placeholder="jane@smithco.com">
              </div>
            </div>
            <label>What's up?</label>
            <textarea rows="4"></textarea>
            <button type="submit" class="radius button">Submit</button>
          </form>
        </div>
      </section>
      <section class="section">
        <h5 class="title"><a href="#panel2">Specific Person</a></h5>
        <div class="content" data-slug="panel2">
          <ul class="large-block-grid-5">
            <li><a href="/cdn-cgi/l/email-protection#82efe3eec2f1e7f0e7ecebf6fbace0e1acf0e7e0"><img src="http://placehold.it/200x200&text=[person]">CEO</a></li>
            <li><a href="/cdn-cgi/l/email-protection#94eefbf1d4e7f1e6f1fafde0edbaf6f7bae6f1f6"><img src="http://placehold.it/200x200&text=[person]">Managing Director</a></li>
            <li><a href="/cdn-cgi/l/email-protection#8ae0ebf3e4efcaf9eff8efe4e3fef3a4e8e9a4f8efe8"><img src="http://placehold.it/200x200&text=[person]">Finance</a></li>
            <li><a href="/cdn-cgi/l/email-protection#c7a3a8a487b4a2b5a2a9aeb3bee9a5a4e9b5a2a5"><img src="http://placehold.it/200x200&text=[person]">Operation</a></li>
            <li><a href="/cdn-cgi/l/email-protection#6e0507020217011b19071a0603170307000a2e1d0b1c0b00071a17400c0d401c0b0c"><img src="http://placehold.it/200x200&text=[person]">John Doe</a></li>
            <li><a href="/cdn-cgi/l/email-protection#d0bcb5b1b6bfbea4b8b5a7b9beb490a3b5a2b5beb9a4a9feb2b3fea2b5b2"><img src="http://placehold.it/200x200&text=[person]">Jane Smith</a></li>
            <li><a href="/cdn-cgi/l/email-protection#4d2f2222260d3e283f2823243934632f2e633f282f"><img src="http://placehold.it/200x200&text=[person]">Abu Bakar</a></li>
            <li><a href="/cdn-cgi/l/email-protection#2d464148486d5e485f4843445954034f4e035f484f"><img src="http://placehold.it/200x200&text=[person]">Ali Kassim</a></li>
            <li><a href="/cdn-cgi/l/email-protection#99f0f7f8ebf8d9feecf0f5fdb7faf6f4e9b7f8f5f5"><img src="http://placehold.it/200x200&text=[person]">Kassim Selamat</a></li>
          </ul>
        </div>
      </section>
    </div>
  </div>
  <div class="large-4 columns">
    <h5>Map</h5>
    <script>
    function initMap() {
      var map = new google.maps.Map(document.getElementById('map'), {
        center: {lat: -33.866, lng: 151.196},
        zoom: 15
      });

      var infowindow = new google.maps.InfoWindow();
      var service = new google.maps.places.PlacesService(map);

      service.getDetails({
        placeId: 'ChIJN1t_tDeuEmsRUsoyG83frY4'
      }, function(place, status) {
        if (status === google.maps.places.PlacesServiceStatus.OK) {
          var marker = new google.maps.Marker({
            map: map,
            position: place.geometry.location
          });
          google.maps.event.addListener(marker, 'click', function() {
            infowindow.setContent(place.name);
            infowindow.open(map, this);
          });
        }
      });
    }
    </script>
    <div id="map"></div>
    <address>
      Jalan Pesisir Pelabuhan 2<br>
      Kampung Sg Ular<br>
      26080 Sungai Karang<br>
      Pahang<br>
      Malaysia<br>
    </address>
  </div>
</div>
