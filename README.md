# Website Link

URL: https://upbeat-hugle-a51ec0.netlify.app/  
Github repo: https://github.com/Todd0554/potfolio_src  

Due to the first part I finished is the website coding, the Github is connected with /src folder. 

# Purpose of this website

To introduce myself, including my ***personal CV***, ***contacting information***, ***daily life*** and ***hobbies***.

# Sitemap
![Sitemap of my website](/docs/Blank%20diagram.png "Sitemap of my website")  
This is the simple sitemap of my website. There are 5 pages totally including Homepage (index.html), Personal CV page(index2.html), About Me page (index3.html), Contact (index4.html) and under the Personal CV page, there is another page of my personal CV in PDF documentation linked with a button in Personal CV page. In addition, every page has the link to my ins, twitter, linkedin and Github.

# Target audience 
To teachers of Coder Academy and future employers.  

# Website introduction
This website is established by HTML5 with SCSS. It is a static website, so there is no Javascript inside of the documentations.  

## 1. Page of Home(index)
![Home](/docs/homepage(index).png)
The picture above is the wireframe of 'Home' page. In this page, a navbar is established with the logo and name on the left side and another 4 link buttons on the right side. The codes are below:
```Html
<!-- navbar -->

        <nav id="navbar">
            <div class="container">
                <div class="heading">
                    <a href="/index.html"><img class="logo" src="/img/mixer-brands.svg" alt="X"></a>
                    <h1><a href="/index.html">XZ's Zoom</a></h1>
                    <ul>
                        <li><a href="/index.html">Home</a></li>
                        <li><a href="/index2.html">Personal CV</a></li>
                        <li><a href="/index3.html">About Me</a></li>
                        <li><a href="/index4.html">Contact</a></li>
                    </ul>
                </div>
            </div>
        </nav>
```


Above the background, 'My name' and 'Position' will slide from left to approximately center by using animation to the target position. In order to keep website responsive, I use the code below:  
```CSS
@media screen and (min-width:1000px){
    @keyframes move1{
        0%{
            width: 20%
        }
        100%{
            width: 55%;
        }
    }

    @keyframes move2{
        0%{
            width: 25%
        }
        100%{
        width: 65%;
        }
    }
}
@media screen and (max-width:1040px) {
    #first-page .name{
        font-size: 0.9rem;
        padding-top: 5%;
    }

    #first-page .position{
        font-size: 0.9rem;
        padding-top: 5%;
    }
    @keyframes move1{
        0%{
            width: 50%
        }
        100%{
            width: 55%;
        }
    }

    @keyframes move2{
        0%{
            width: 60%
        }
        100%{
        width: 65%;
        }
    }
}

@media screen and (max-width:350px) {
    #first-page .name{
        font-size: 0.7rem;
        padding-top: 5%;
    }

    #first-page .position{
        font-size: 0.7rem;
        padding-top: 5%;
    }
    #navbar a{
        font-size: 0.7rem;
    }
    @keyframes move1{
        0%{
            width: 50%
        }
        100%{
            width: 55%;
        }
    }

    @keyframes move2{
        0%{
            width: 60%
        }
        100%{
        width: 65%;
        }
    }
}
```  
On the bottom, 4 icons which links my *Linkedin*, *Twitter*, *ins* and *Github* are arranged in a row. I give each of them an 360deg rotating animation when the cursor ***hover*** on it. At last there is the footer under them.

## 2. Page of Personal CV(index2)
![Personal_CV](/docs/Personal%20CV%20page(index2).png)
This is the 'Personal CV' page which is relatively simple. I use ***div*** to set the text of my *studying experience*, *competency* and *other certificate* I own. 

There is a button linking with my *Personal CV in PDF* under the text.


## 3. Page of About Me(index3)
![About_me](/docs/About%20me(index3).png)
The image above is the third page of this website, which introduce my current situation. Under the navbar, there is a simple personal introduction and a photo(here is just ***Homer Simpson***) of me. Then is the hobbies section which includes three cards with image and a short description.  
```Html
 <section id="threecard">
        <div class="container">
            <h1>My Hobbies</h1>
            <div class="card">
                <img src="./img/pexels-pixabay-51323.jpg" alt="#">
                <h2>Music</h2>
                <p>Music is one of my relaxing styles. I like playing guitar, bass, blues-harmonica and many other music instruments. Sometimes, I record the song with my friends online.</p>
            </div>
            <div class="card">
                <img src="./img/pexels-pixabay-361184.jpg" alt="#">
                <h2>Cooking</h2>
                <p>It is not so much cooking as eating. No one don't like delicious food. I'm no exception. Because of covid, cooking has already become one of my favourite entertainment.</p>
            </div>
            <div class="card">
                <img src="./img/pexels-andrei-tanase-1271619.jpg" alt="#">
                <h2>Traveling</h2>
                <p>Including hiking, finishing, camping and so on. Traveling always can bring me a great mood, which also improves my working efficiency. BTW, my next destination is New Zealand.</p>
            </div>
        </div>
    </section>
```    



Finally, there are 5 blog screenshoots of my life. I also give each image a shadow on the right and bottom side, which makes the website more 3D. Moreover, these images are also responsive on different devices with the code below:
```CSS
@media screen and (max-width:1400px) {
    #threecard .container .card{
        width: 45%;
    }
}

@media screen and (max-width: 1000px) {
    #threecard .container .card{
        width: 80%;
    }
}
// responsive settings of blog section

@media screen and (max-width:770px){
    #blog .container .box{
        width: 100%;
    }
    #blog{
        height: 3300px;
    }
}

@media screen and (max-width:500px){
    #blog .container .box{
        width: 100%;
    }
    #blog{
        height: 2700px;
    }
}
```  
## 4. Page of Contact(index4)
![Contact](/docs/Contact(index4).png)
'Contact' section is the last page of this website except the PDF of personal CV. In this page, the visitor can contact me by using the input boxes and textarea. 

## 5. Other Features
A special icon is used in title of every page, which is from Font Awesome. Another font from Google font is also used for this website. 

## 6. Deployment
This website is connected with the Github repo and deployed on Netlify. Of course, the Netlify is also linked with Github, so if I update some parts of the website and push them into Github, the website will also be updated in several minutes.

## 7. Responsive Screenshoots
Here are the screenshoots of my website in different device.
![Homepage](/docs/Screen%20Shot%202022-03-18%20at%2018.06.36.png)
![PersonalCV](/docs/Screen%20Shot%202022-03-18%20at%2018.05.40.png)
![AboutMe](/docs/Screen%20Shot%202022-03-18%20at%2018.06.11.png)
![Contact](/docs/Screen%20Shot%202022-03-18%20at%2018.06.57.png)
# Conclusion
To sum up, this is a simple static website of my introduction. This markdown document give a concise description of the website including my studying experience, CV, contact information and other social media links. 