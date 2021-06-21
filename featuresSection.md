# Features Section
now its time to create feature section of our website

from now we will be working inside our features section 

our first task is to add custom logo using [lineAwesome](https://icons8.com/line-awesome)

after selecting the and modifying the icon of our choice we can add them to our index.html

Initially our code look like this with features section having no styling in styles.css

```
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
```

## Modifications
Now we have a single row as a Whole feature section.
we have three divs in our row with each div having a icon h3 and a paragraph tag

To make it responsive we will add col-lg-4 because i want, when in large screen size 3 rows taking up the space 

For that we will 12/3 = 4 so the class will be col-lg-4

### End result

```
  <section id="features">
    <!-- Features -->
    <div class="row">
      <div class="col-lg-4">
      <img src="https://img.icons8.com/ios-glyphs/90/000000/globe--v1.png" />
      <h3>All in one</h3>
      <p>No need to switch between multiple apps</p>
    </div>
          <div class="col-lg-4"><img src="https://img.icons8.com/ios-glyphs/90/000000/globe--v1.png" />
            <h3>All in one</h3>
            <p>No need to switch between multiple apps</p>
          </div>
                <div class="col-lg-4"><img src="https://img.icons8.com/ios-glyphs/90/000000/globe--v1.png" />
                  <h3>All in one</h3>
                  <p>No need to switch between multiple apps</p>
                </div>
    </div>
  </section>
```

Still our features section is not similar to the chats website
what it lacking is Styling in Styles.css

first We add a custom class named feature-box to all three rows 
now in styles.css we will add
`.feature-box{
  text-align: center;
  padding: 7% 15%;
}
` 
This will make our contents center aligned with padding 

Now we will add background color in our feature section using css

for that we will target our id which is #features and add extra properties 
`#features{
  background-color: #3282b8;
  padding: 7% 15%;
`

Now will add some more css like
```
h2{
  font-family: 'Montserrat',Semi-bold 600;
}
h3{
  color: white;
  font-family: 'Montserrat',Semi-bold 600;
  font-weight:bold;
}
p{
  color: #bbe1fa;
  font-family: 'Montserrat',Regular 400;
  font-weight:normal;
}
```

# Testimonials section 




