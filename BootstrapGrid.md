## Lets see this in action
head over to vs code and setup a sample index.html file with bootstrap linked to it

copy pate this code

```
<div class="row">                
<div class="col" style="background-color: red; border: 1px solid;">col</div>
</div>
```

as we can see the red colum is taking up the entire width of the Screen 

*The interesting thing about class ***col**** is

It divides up the row to as many sections as they need  in order to distribute all of the columns it needs

now if we have two divs with class **col** inside a row then both will take 50% of screen 

if we add third div like this
```
 <div class="row">
                <div class="col" style="background-color: red; border: 1px solid;">col</div>
                <div class="col" style="background-color: red; border: 1px solid;">col</div>
                <div class="col" style="background-color: red; border: 1px solid;">col</div>
            </div>

```
Now wht if i want to add the colum that only took up half of the width on the screen  

Now we create a new Div just below the previous one for the sake of reference  

``` 
<div class="row">
<div class="col-6" style="background-color: green; border: 1px solid;">col-6</div>
</div>
```
now in this you can see that our column takes only 50% of the width of the screen

Its clear that we can use numbers to specify how much of the row to take up by a col   

**The total units for a single row is 12**

this means that

-12/6 =2 or half of the row

-12/3 =4 or quarter of the row

-12/2 =6 or sixth of the row

-12/1 =12 or only 1part of the 12 sized row

```
<div class="row">
                <div class="col-6" style="background-color: green; border: 1px solid;">col-6</div>
                <div class="col-3" style="background-color: green; border: 1px solid;">col-6</div>
                <div class="col-2" style="background-color: green; border: 1px solid;">col-6</div>
                <div class="col-1" style="background-color: green; border: 1px solid;">col-6</div>
</div>

```

The problem with the method above is, if we change the size of screen nothing changes it remains the same   

So how to get airbnb effects that we saw earlier

Solution to this problem is adding a responsive colum 

The responsive colum have a class of  "col-md-6" in this (md) defines the device width like medium, small, large

--- 

**col-md-6** stands for we should have **six** units **colum** on any size from **medium** to upwards but anything **smaller** than medium will take up the **full width**

```
<div class="row">
                <div class="col-md-6" style="background-color: blue; border: 1px solid;">col-md-6</div>
                <div class="col-md-6" style="background-color: blue; border: 1px solid;">col-md-6</div>
</div>
```
Your final code must look like this
```
            <div class="row">
                <div class="col" style="background-color: red; border: 1px solid;">col</div>
                <div class="col" style="background-color: red; border: 1px solid;">col</div>
                <div class="col" style="background-color: red; border: 1px solid;">col</div>
            </div>
            <div class="row">
                <div class="col-6" style="background-color: green; border: 1px solid;">col-6</div>
                <div class="col-3" style="background-color: green; border: 1px solid;">col-6</div>
                <div class="col-2" style="background-color: green; border: 1px solid;">col-6</div>
                <div class="col-1" style="background-color: green; border: 1px solid;">col-6</div>
            </div>
            <div class="row">
                <div class="col-md-6" style="background-color: blue; border: 1px solid;">col-md-6</div>
                <div class="col-md-6" style="background-color: blue; border: 1px solid;">col-md-6</div>
            </div>

```

Now if we delete
```
                <div class="col-2" style="background-color: green; border: 1px solid;">col-6</div>
                <div class="col-1" style="background-color: green; border: 1px solid;">col-6</div>
```

And change green col-3 to col-6 

**then we end up having**

``` <section id="GridSystem">
            <div class="row">
                <div class="col" style="background-color: red; border: 1px solid;">col</div>
                <div class="col" style="background-color: red; border: 1px solid;">col</div>
                <div class="col" style="background-color: red; border: 1px solid;">col</div>
            </div>
            <div class="row">
                <div class="col-6" style="background-color: green; border: 1px solid;">col-6</div>
                <div class="col-6" style="background-color: green; border: 1px solid;">col-6</div>
            </div>
            <div class="row">
                <div class="col-md-6" style="background-color: blue; border: 1px solid;">col-md-6</div>
                <div class="col-md-6" style="background-color: blue; border: 1px solid;">col-md-6</div>
            </div>
        </section>
```

three rows looking almost same 
- first three(red) col are taking  4 parts of the row 
- second two(green) col are taking 6 parts of the row(Non responsive)
- third two(blue) col are  also taking 6 parts of the row but as long it is in tablet size or larger as soon as we switch to smaller size it takes 100% of the row
---
### What if we need more specific results ?
like in desktop size it must have
- [ ] four columns on desktop
- [ ] three columns on tablet
- [ ] two columns on mobile 

### Lets get Started
first we add two more responsive divs (blue columns) to make it four

Then we start with the simplest, 

So we want four columns in desktop
so **12/4 = 3** and we can specify screen size by keyword **lg** and 3

and change all the divs to this format

```
            <div class="row">
                <div class="col-lg-3" style="background-color: blue; border: 1px solid;">col-lg-3</div>
                <div class="col-lg-3" style="background-color: blue; border: 1px solid;">col-lg-3</div>
                <div class="col-lg-3" style="background-color: blue; border: 1px solid;">col-lg-3</div>
                <div class="col-lg-3" style="background-color: blue; border: 1px solid;">col-lg-3</div>
            </div>
```
But now on tablet and mobile we can see they take 100%of the width 

thats not we want 

we Want
So we want three columns in tablet
so **12/3 = 4** and we can specify screen size by keyword **md** and 4

so we add another rule in blue col which is--

**col-md-4**

Now our code must look like 
```            <div class="row">
                <div class="col-lg-3 col-md-4" style="background-color: blue; border: 1px solid;">col-lg-3</div>
                <div class="col-lg-3 col-md-4" style="background-color: blue; border: 1px solid;">col-lg-3</div>
                <div class="col-lg-3 col-md-4" style="background-color: blue; border: 1px solid;">col-lg-3</div>
                <div class="col-lg-3 col-md-4" style="background-color: blue; border: 1px solid;">col-lg-3</div>
            </div>

```

Now in mobile its still taking 100%of the width

we Want
So we want two columns in mobile
so **12/2 = 6** and we can specify screen size by keyword **sm** and 6

so we add another rule in blue col which is--

**col-sm-6**
Final code must look like
```
            <div class="row">
                <div class="col-lg-3 col-md-4 col-sm-6" style="background-color: blue; border: 1px solid;">col-lg-3</div>
                <div class="col-lg-3 col-md-4 col-sm-6" style="background-color: blue; border: 1px solid;">col-lg-3</div>
                <div class="col-lg-3 col-md-4 col-sm-6" style="background-color: blue; border: 1px solid;">col-lg-3</div>
                <div class="col-lg-3 col-md-4 col-sm-6" style="background-color: blue; border: 1px solid;">col-lg-3</div>
            </div>

```

# **Home-work**

Create another row below these three and give it a different color so that it look different, make this set responsive and

1. On the larger desktop size it must have six columns per row
2.  On the tablet or medium size it must have 4 columns per row
3. On the Mobile it should take 100% of the row

For help refer [Docs-bootstrap](https://getbootstrap.com/docs/5.0/layout/grid/)
