# Styling header section
 make our first section a six unit column so that it takes up half of the screen.The image must also takes another six unit colum so it takes up the right side 50 percent of the screen 

But on tablet or mobile size it must take 100% of the page.

##background Color

Now before moving ahead we must style our webpage 

so the background color of our header section is background-color: #0f4c75; 

```
#title{
    background-color: #0f4c75;
}
```

##Header/Title section

So we want to make download button take up 50% of the width on the left and the image of the phone also take up 50%  of the width on the right on the large Desktop size.

```
    <div class="row">
      <div class="col-lg-6">
<h1>Get your own private chat room</h1>
<button>Sign up now</button>
      </div>
    
    
    <div class="col-lg-6">
    <img src="images\mobile-employees-us-1588077320.png" alt="">
    </div>


  </div>
  </section>
```
## Fonts
The next thing we want is change our text font styling

Lets open google and go to [googleFonts](https://fonts.google.com/) 

Now we will use google fonts cdn similar to Bootstrap


first is Montserrat for our website

After applying google fonts CDN we want
our h1 to have a font-family of Montserrat , bold 700 with size of 4rem and line height 1.5rem

For rest of our html body we need Montserrat semi-bold 600 and regular 400
```
body{
   font-family: 'Ubuntu', sans-serif;
}

h1{
    color: #bbe1fa;
    font-family: 'Montserrat', Bold 700;
    font-size: 4rem;
    line-height: 1.5rm;
}
```

# Bootstrap Container 
Containers are the basic building blocks in lot of the components in Bootstrap 

As in example of grid system all of these grids are contained inside a container 

```
<div class="container">
  <div class="row">
    <div class="col-sm">
      One of three columns
    </div>
    <div class="col-sm">
      One of three columns
    </div>
    <div class="col-sm">
      One of three columns
    </div>
  </div>
</div>
```
[Bootstrap containers](https://getbootstrap.com/docs/4.1/layout/overview/#containers)

## Example
In vscode open sample section 
and index.html 

now we will se diffrence between non container div container div and fluid container div
```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css"
        integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">

    <title>Hello, world!</title>
</head>

<body>
    <div style="background-color: aqua;">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
        aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis
        aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
        occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
        aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis
        aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
        occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>
        <div class="container" style="background-color: red;">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
                magna
                aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
                consequat. Duis
                aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
                occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        </div>


        <div class ="container-fluid"style="background-color: yellow;">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
                magna
                aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
                consequat. Duis
                aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
                occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
                aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis
                aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
                occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        </div>


    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"
        integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js"
        integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49"
        crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"
        integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy"
        crossorigin="anonymous"></script>
</body>

</html>
```

#### So after enclosing our whole header section or navigation bar heading images and button inside a fluid container the code must look like this

```
<!doctype html>
<html lang="en">

<head>
  <!-- Required meta tags -->
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Chats</title>
  <link rel="icon" href="favicon-16x16.png">
  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link
    href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,600;0,900;1,600;1,800&family=Ubuntu&display=swap"
    rel="stylesheet">
  <link rel="stylesheet" href="css\styles.css">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.1/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-+0n0xVW2eSR5OomGNYDnhzAbDsOXxcvSN1TPprVMTNDbiYZCxYbOOl7+AMvyTG2x" crossorigin="anonymous">
</head>
<body>
  <section  id="title">
     <!-- Title -->
    <div class="container-fluid">
    <nav class=" color-change navbar navbar-expand-lg navbar-dark">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Chats</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
          aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Features</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Download</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
<div class="row">
    <div class="col-lg-6">
      <h1>Get your own private chat room</h1>
      <button>Sign up now</button>
    </div>
    <div class="col-lg-6">
      <img src="images\mobile-employees-us-1588077320.png" alt="">
    </div>
</div>
</div>



        






  </section>

  
  <section id="features">
    <!-- Features -->
  </section>



  

  <section id="testimonials">
    <!-- Testimonials -->

  </section>

  
  <section id="press">
    <!-- Press -->
  </section>

  
  <section id="cta">
    <!-- Call to Action -->

  </section>


  <section id="footer">
    <!-- footer -->
    </footer>

  </section>
  <!-- JavaScript Bundle with Popper -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.1/dist/js/bootstrap.bundle.min.js"
    integrity="sha384-gtEjrD/SeCtmISkJkNUaaKMoLD0//ElJ19smozuHV6z3Iehds+3Ulb9Bn9Plx0x4" crossorigin="anonymous"></script>
</body>
</html>

```
After that if we headover to styles.css 
we can modify our default container

we add padding to container-fluid

`
.container-fluid{
    padding: 3% 15%;
    }
`

Afte modifying this we have a new challange which is our bootstrap 

if we look through documentation we will find a seprate section for buttons in bootstrap [BootstrapDOC](https://getbootstrap.com/docs/4.1/components/buttons/)

if you notice we just have to add few classs and our styled button is ready

Not only the design we can also change the size of the Buttons

```
<div class="row">
    <div class="col-lg-6">
      <h1>Get your own private chat room</h1>
      <button class="btn btn-dark btn-lg">Sign up now</button>
    </div>
    <div class="col-lg-6">
      <img src="images\mobile-employees-us-1588077320.png" alt="">
    </div>
</div>
```
Still one thing is missing the logo of google 
lets se how to add it in our Code

Headover to [LineAwsome](https://icons8.com/line-awesome)
now if go on getting started we can see the CDN links copy pate it into our html code

Afte copy pasting the cdn select the icon of ypur own choice 
click on it choose a custom size then paste it inside the button or the section you want 

the position of the link will also decicde the positon of icon inside a element
```
 <button   class="btn btn-dark btn-lg">Sign up now <img src="https://img.icons8.com/material-sharp/24/000000/google-logo.png" /></button>
``` 
##  CSS Styling
Now lets begin some final touchups in our html using css

```
.navbar{
  padding-bottom: 2.5rem;
}
.navbar-brand{
  font-family: 'Ubuntu' Bold 700;
  font-size: 2.5rem;
  font-weight: bold;
}
.nav-item{
  padding: 0 18px;
}
.nav-link{
  font-size: 1.25rem;
  font-family: "Montserrat",sans-serif;
}
```
And then give our button a unique class sign-up-button
# index.html 19/06
```
<!doctype html>
<html lang="en">

<head>
  <!-- Required meta tags -->
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Chats</title>
  <link rel="icon" href="favicon-16x16.png">
  <link rel="stylesheet"
    href="https://maxst.icons8.com/vue-static/landings/line-awesome/font-awesome-line-awesome/css/all.min.css">
  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link
    href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,600;0,900;1,600;1,800&family=Ubuntu&display=swap"
    rel="stylesheet">
  <link rel="stylesheet" href="css\styles.css">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.1/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-+0n0xVW2eSR5OomGNYDnhzAbDsOXxcvSN1TPprVMTNDbiYZCxYbOOl7+AMvyTG2x" crossorigin="anonymous">
</head>
<body>
  <section  id="title">

    <div class="container-fluid">
     <!-- Title -->
    <nav class=" color-change navbar navbar-expand-lg navbar-dark">
      <div class="container-fluid">
        <a class="navbar-brand" href="#"><h1>Chats</h1></a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
          aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Features</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Download</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>




<div class="row">
    <div class="col-lg-6">
      <h1>Get your own private chat room</h1>
      <button class="btn btn-dark btn-lg">Sign up now <img src="https://img.icons8.com/fluent/24/000000/google-logo.png"/></button>
    </div>
    <div class="col-lg-6">
      <img src="images\mobile-employees-us-1588077320.png" alt="">
    </div>
</div>
</div>
</section>

 


  <section id="features">
    <!-- Features -->
    <div class="row">
      <div class="col"><img src="https://img.icons8.com/ios-glyphs/90/000000/globe--v1.png" />
      <h3>All in one</h3>
      <p>No need to switch between multiple apps</p>
    </div>
          <div class="col"><img src="https://img.icons8.com/ios-glyphs/90/000000/globe--v1.png" />
            <h3>All in one</h3>
            <p>No need to switch between multiple apps</p>
          </div>
                <div class="col"><img src="https://img.icons8.com/ios-glyphs/90/000000/globe--v1.png" />
                  <h3>All in one</h3>
                  <p>No need to switch between multiple apps</p>
                </div>
    </div>
  </section>



  

  <section id="testimonials">
    <!-- Testimonials -->

  </section>

  
  <section id="press">
    <!-- Press -->
  </section>

  
  <section id="cta">
    <!-- Call to Action -->

  </section>


  <section id="footer">
    <!-- footer -->
    </footer>

  </section>
  <!-- JavaScript Bundle with Popper -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.1/dist/js/bootstrap.bundle.min.js"
    integrity="sha384-gtEjrD/SeCtmISkJkNUaaKMoLD0//ElJ19smozuHV6z3Iehds+3Ulb9Bn9Plx0x4" crossorigin="anonymous"></script>
</body>
</html>

```


# styles.css
```
#title{
    background-color: #0f4c75;
}
body{
   font-family: 'Ubuntu', sans-serif; 
}

h1{
    color: #bbe1fa;
    font-family: 'Montserrat', Bold 700;
    font-size: 4rem;
    line-height: 1.5rem;
}
.container-fluid{
    padding: 3% 15%;
}

.navbar{
  padding-bottom: 2.5rem;
}
.navbar-brand{
  font-family: 'Ubuntu' Bold 700;
  font-size: 5rem;
  font-weight: bold;
}
.nav-item{
  padding: 0 18px;
}
.nav-link{
  font-size: 1.25rem;
  font-family: "Montserrat",sans-serif;
}

```

chats for reference[completeChats](https://amolchourasia27.github.io/WebDev_projects_landing_page/)