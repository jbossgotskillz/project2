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
    <link rel="stylesheet" type="text/css" href="./css_files/project2.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@400..700&display=swap" rel="stylesheet">

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

    
    <div class="nav-item my-4">
        <a class="btn btn-primary" href="#backtothetop" role="button">Return to Dojo Entrance</a>
    </div>

    <!--Tutorial-->
    
    <div class="container my-4" id="tutorial">
      <h1 class="title text-center">Tutorial Room</h1>
      <p>Before entering the CrazyNinja dojo, we recommend you to take a tour of our site.  Doing this will help you get an idea of how everything works.  Plus, while on the tour, you may feel the fire of the almighty 
        dragon burn in your soul.  As scary as that sounds, there is no need to panic.  You will not face death.  Rather, when the dragon breathes its fire upon you, you experience a spiritual awakening.  This is the 
        way of CrazyNinja.  In other words, your passion will grow, and you will feel more compelled to train at the CrazyNinja school.  Go ahead and take the tour of you wish.  If you have questions, then you can 
        reach out to the grand master, who will be more than happy to answer your questions.</p>

        
    <form class="contact-form my-4 needs-validation" 
          action="#"
          method="POST"
          novalidate>
          <div class="form-group row">
            <div class="col-3 offset-3" >

                <label class="container-fluid p-0">
                    First Name
                    <input type="text" class="form-control" id="validationServerUsername" 
                        placeholder="Enter your first name"
                        required>
                    <span class="invalid-feedback">
                        You must enter a name.
                    </span>
                    <span class="valid-feedback">
                        Well done.
                    </span>
                </label>
                
            </div>
            <div class="col-3">

              <label class="container-fluid p-0">
                  Last Name
                  <input type="text" class="form-control" id="validationServerUsername2" 
                        placeholder="Enter your last name"
                        required>
                    <span class="invalid-feedback">
                        You must enter a name.
                    </span>
                    <span class="valid-feedback">
                        Well done.
                      </span>
              </label>
          </div>
        </div>
        <div class="form-group row">
            <div class="col col-md-6 offset-md-3">
                <label class="container-fluid p-0">
                    Email
                </label>
                <input type="email" 
                    class="form-control" 
                    id="password" 
                    placeholder="Enter your email" 
                    required>
                    <span class="invalid-feedback">
                      You must use a valid email address.
                    </span>
                  <span class="valid-feedback">
                      Well done.
                  </span>
            </div>
        </div>
        <div class="form-group row">
            <div class="col col-md-6 offset-md-3">
                <label for="textarea">
                    Message
                </label>
                <textarea class="form-control" 
                        id="textarea" 
                        rows="3"></textarea>
            </div>
        </div>
        <div class="form-group row my-4">
            <div class="col col-md-6 offset-md-3 text-center">
                <button type="submit" 
                        class="btn btn-primary">
                    Speak to Grand Master
                </button>            
            </div>
          </div>
  
          </form>

        </div>
      
      <div class="form-group row justify-content-center my-4">
            <button type="button" aria-current="page" class="btn btn-primary col-3">Take Tour</button>
        </div>

        
    <div class="nav-item my-4">
        <a class="btn btn-primary" href="#backtothetop" role="button">Return to Dojo Entrance</a>
    </div>
        
    <!--Image Gallery-->

    <div class="container my-4" id="image-gallery">  
      <h1 class="title text-center">Image Gallery Room</h1>
      <p>This dojo offers a lot of images to choose from.  However, getting them requires intense training.  Boost your skills as a ninja by searching for and capturing the images you seek, and become legendary.</p>
    
      <form action="#image-gallery" class="js-repo-form text-center" method="GET">    <!--<form action="#"-->
        <label>
            Search Category:
            <input type="text" name="repo-name" placeholder="Select your training">
        </label>
        <button type="submit" aria-current="page" class="btn btn-primary">Begin</button>
      </form>
      <section class="js-repo-container"></section>
    </div>

    
    <div class="nav-item my-4">
        <a class="btn btn-primary" href="#backtothetop" role="button">Return to Dojo Entrance</a>
    </div>
    
    <!--Registration-->

    <div class="container" id="registration">
      <h1 class="title text-center" >Registration Room</h1>
      <p>Want to join the CrazyNinja school?  Sign up here.</p>
    </div>
      
    <div class="nav-item my-4">
        <a class="btn btn-primary" href="#backtothetop" role="button">Return to Dojo Entrance</a>
    </div>


    <nav class="navbar justify-content-center">
      <div class="end text-center">
        <p>POWERED BY DRAGON FIRE</p>
        <p>TRAINED BY GIPHY</p>
      </div>
    </nav>
    
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>


</body>

    </html>

# project2
