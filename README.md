Name:  Jordan Woodard

Overview:  This is a school project for an image search app that I made called "CrazyNinja".  The concept for the CrazyNinja app centers around building a "ninja school" that "teaches" its "students" how to find images for their projects.  Therefore, I used a theme based on ninjas and the art of ninjutsu (or ninja arts).

Details:  CrazyNinja contains an API search engine called Giphy.  There are four sections on the app:  Home, Tutorial, Image Gallery, and Registration.  A navigation bar features links for each section, while the ends of each section feature buttons that take users back to the navigation bar.  The image search is done under the Tutorial section.  Meanwhile, there are two other forms:  one under the Tutorial section and one under the Registration section.  Both of them can be interacted with.

Technologies:  html, css, js

Improvements:  



<!doctype html>

    <html lang="en">

<head>
    
    <title>Crazy Ninja</title>

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">

</head>

<body>
    
  <!--navbar-->

  <nav class="navbar navbar-expand-lg d-flex">
    <div class="row container-fluid" id="backtothetop">
    <div class="col-8">
      <p class="navbar-brand my-auto">CrazyNinja</p>
    </div>
    <div class="col-1">
      <div class="nav-item"></div>
        <a class="nav-link active" aria-current="page" href="#main">Main</a>
    </div>
    <div class="col-1">
      <div class="nav-item"></div>
        <a class="nav-link" href="#tutorial">Tuturial</a>
    </div>
    <div class="col-1">
      <div class="nav-item"></div>
        <a class="nav-link" href="#image-gallery">Image Gallery</a>
    </div>
    <div class="col-1">
      <div class="nav-item"></div>
        <a class="nav-link" href="#registration">Registration</a>
    </div>
    </div>
  </nav>



  
    <!--Main-->

    <div class="container my-4">
      <h1 class="title text-center" id="main">Main Room</h1>
      <p>Welcome to CrazyNinja, where aspiring ninja warriors come to master the art of image hunting.  We understand how difficult and frustrating it can be as a content creator to find the perfect images for 
        your web project, so we at CrazyNinja are honored to show you the way.  If you are interested in browsing through our dojo, then enter as you wish.  In addition, if you like what we have to offer and would
        like to become a member of the CrazyNinja school, then you must register to create an account.  Meanwhile, you may walk away from our dojo at any time.  Oh...and as a means of assurance, we will not send our 
        ninja assassins after you over your treachery, so do not be concerned.</p>
        <!--add image-->
    </div>
  
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>

</body>

    </html>

# project2
