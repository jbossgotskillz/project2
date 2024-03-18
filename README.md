Name:  Jordan Woodard

Overview:  This is a school project for an image search app that I made called "CrazyNinja".  The concept for the CrazyNinja app centers around building a "ninja school" that "teaches" its "students" how to find images for their projects.  Therefore, I used a theme based on ninjas and the art of ninjutsu (or ninja arts).

Details:  CrazyNinja contains an API search engine called Giphy.  There are four sections on the app:  Home, Tutorial, Image Gallery, and Registration.  A navigation bar features links for each section, while the ends of each section feature buttons that take users back to the navigation bar.  The image search is done under the Tutorial section.  Meanwhile, there are two other forms:  one under the Tutorial section and one under the Registration section.  Both of them can be interacted with.

Technologies:  html, css, js

Improvements:  spend more time understanding Javascript, customize alert boxes, figure out how to build a better search engine


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
    <link rel="stylesheet" href="./project2.css">

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

    <div class="banner-container justify-content-center d-flex">
      <img src="./crazy_ninja.jpg"  height="300" alt="banner">
      <img src="./crazy_ninja2.jpg"  height="300" alt="banner2">
      <img src="./crazy_ninja3.jpg"  height="300" alt="banner3">
    </div>

    
    <!--Main-->

    <div class="container my-4">
      <h1 class="title text-center" id="main">Main Room</h1>
      <p>Welcome to CrazyNinja, where aspiring ninja warriors come to master the art of image hunting.  We understand how difficult and frustrating it can be as a content creator to find the perfect images for 
        your web project, so we at CrazyNinja are honored to show you the way.  If you are interested in browsing through our dojo, then enter as you wish.  In addition, if you like what we have to offer and would
        like to become a member of the CrazyNinja school, then you must register to create an account.  Meanwhile, you may walk away from our dojo at any time.  Oh...and as a means of assurance, we will not send our 
        ninja assassins after you over your treachery, so do not be concerned.</p>
      <img src="./dojo2.jpg" class="d-block" alt="dojo">
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
      
      <div class="form-group row justify-content-center my-4">
        <button class="btn btn-primary col-3" onclick="schoolTour()">Take tour</button>
</div>

<script>
function schoolTour() {
  alert("Due to an attack by ninjas from a rival school, no tours are being allowed at this time.  We apologize for the inconvenience.");
}
</script>

        
        <img src="./eastern_dragon.jpg" class="d-block" alt="eastern dragon">

    <form class="contact-form my-4 needs-validation" 
          action="#tutorial"
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

          <div class="nav-item my-4">
            <a class="btn btn-primary" href="#backtothetop" role="button">Return to Dojo Entrance</a>
          </div>
  
    <!--Image Gallery-->

    <div class="container my-4" id="image-gallery">  
      <h1 class="title text-center">Image Gallery Room</h1>
      <p>This dojo offers a lot of images to choose from.  However, getting them requires intense training.  Boost your skills as a ninja by searching for and capturing the images you seek, and become legendary.</p>
    
      <form action="#image-gallery" class="js-repo-container text-center" method="GET">    <!--<form action="#"-->
        <label>
            Search Category:
            <input type="text" name="repo-name" placeholder="Select your training">
        </label>
        <button type="submit" aria-current="page" class="btn btn-primary">Begin</button>

      </form>
     

      
           
      <div class="header"> 
        <h1>Gif Search Engine</h1> 
      </div> 
      <div class="container container-padding50"> 
        <input type="text" class="js-userinput  
          container-textinput" /> 
        <button class="js-go container-button"> 
          Search! 
        </button> 
      </div> 
      <div class="container  
        container-padding50 js-container"> 
      </div>
  

    </div>

    
<style> 
    
  body { 
    width: 80%; 
    max-width: 1024px; 
    margin: 0 auto; 
  } 
    
  .header { 
    padding: 100px 50px 50px 40px; 
    position: relative; 
    top: 50px; 
  } 
    
  h1 { 
    font-weight: bold; 
    font-style: normal; 
    font-family: "Times New Roman"; 
    font-size: 72px; 
    color: #090; 
    text-align: center; 
  } 
    
  .container-padding50 { 
    padding: 80px 0px 0px 30px; 
  } 
    
  .container-textinput { 
    width: 70%; 
    display: inline-block; 
    padding: 16px; 
    font-size: 20px; 
    font-family: Helvetica, sans-serif; 
  } 
    
  .container-button { 
    width: 20%; 
    display: inline-block; 
    padding: 16px; 
    background-color: green; 
    color: white; 
    font-size: 20px; 
    font-family: Helvetica, sans-serif; 
    
    border: 1px solid green; 
    border-radius: 5px; 
  } 
    
  .container-image { 
    width: 30%; 
    display: block; 
    float: left; 
    margin-right: 3%; 
  } 
    
  </style>




  
    
    <div class="nav-item my-4">
      <a class="btn btn-primary" href="#backtothetop" role="button">Return to Dojo Entrance</a>
    </div>
    
    <!--Registration-->

    <div class="container my-4" id="registration">
      <h1 class="title text-center" >Registration Room</h1>
      <p>Want to join the CrazyNinja school?  Sign up here.</p>
    


      <form class="contact-form my-4 needs-validation" 
      action="#registration"
      method="POST"
      novalidate>
      <div class="form-group row">
        <div class="col-3 offset-3" >

            <label class="container-fluid p-0">
                Username
                <input type="text" class="form-control" id="validationServerUsername" 
                    placeholder="Enter your first name"
                    required>
                <span class="invalid-feedback">
                    You must enter a valid username.
                </span>
                <span class="valid-feedback">
                    Well done.
                </span>
            </label>
            
        </div>
        <div class="col-3">

          <label class="container-fluid p-0">
              Password
              <input type="text" class="form-control" id="validationServerUsername2" 
                    placeholder="Enter your last name"
                    required>
                <span class="invalid-feedback">
                    You must enter a valid password.
                </span>
                <span class="valid-feedback">
                    Well done.
                  </span>
          </label>
      </div>
    </div>

    <div class="form-group row my-4">
        <div class="col col-md-6 offset-md-3 text-center">
            <button type="button" class="btn btn-primary" onclick="joinDojo()">Join Us</button>
            <p id="membership"></p>
        </div>
      </div>

      </form>

<script>
function joinDojo() {
  var txt;
  if (confirm("Judging by your response, you seem to possess great courage.  However, courage alone can only get you so far.  Skill is also important, and honing your skill requires discipline.  You must be prepared to work countless hours and be willing to make countless sacrifices.  So before you join us, ask yourself.  Are you really sure that you want to become a member of our dojo?")) {
    txt = "Very well.  Let's see what you got!";
  } else {
    txt = "No problem.  Come back when you are truly ready.";
  }
  document.getElementById("membership").innerHTML = txt;
}
</script>

      </div>

    <nav class="navbar justify-content-center">
      <div class="end text-center">
        <p>POWERED BY DRAGON FIRE</p>
        <p>TRAINED BY GIPHY</p>
      </div>
    </nav>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
    
    <script src="https://code.jquery.com/jquery-3.5.1.js" integrity="sha256-QWo7LDvxbWT2tbbQ97B53yJnYU3WhH/C8ycbRAkjPDc=" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>

    <script src="./project2.js"></script>
</body>

    </html>
