---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home
---


<!-- Image slider -->
<div id="slides" class="carousel slice" data-ride="carousel">
    <ul class="carousel-indicators">
        <li data-target="#slides" data-slide-to="0" class="active"></li>
        <li data-target="#slides" data-slide-to="1"></li>
        <li data-target="#slides" data-slide-to="2"></li>
    </ul>
    <div class="carousel-inner">
        <div class="carousel-item active">
            <img src="{{site.url}}/images/background.jpg">
            <div class="carousel-caption">
                <h1 class="display-2">Doan Nguyen</h1>
                <h3>#Thinker. #(0.5)Introvert . #Mechatronics . #AI. #Vlogger. #Writer</h3> 
                <button type="button" class="btn btn-primary btn-lg"> About Me!</button>
            </div>
        </div>
        <div class="carousel-item">
            <img src="{{site.url}}/images/background2.png">
            <div class="carousel-caption">
                <h1 class="display-2">Doan Nguyen</h1>
                <h3>#Thinker. #(0.5)Introvert . #Mechatronics . #AI. #Vlogger. #Writer</h3> 
                <button type="button" class="btn btn-primary btn-lg"> About Me!</button>
            </div>
        </div>
        <div class="carousel-item">
            <img src="{{site.url}}/images/background3.jpg">
            <div class="carousel-caption">
                <h1 class="display-2">Doan Nguyen</h1>
                <h3>#Thinker. #(0.5)Introvert . #Mechatronics . #AI. #Vlogger. #Writer</h3> 
                <button type="button" class="btn btn-primary btn-lg"> About Me!</button>
            </div>
        </div>
    </div>
</div>

<!-- Some thoughts -->
<div class="container-fluid padding">
<div class="row welcome text-center jumbotron padding">
    <div class="col-12">
        <p><i>It'd been three years since when I wanted to have my address. Tried several hosts: Google Blogger, WordPress, and some local brands but got frustrated when looking on their restricted or pre-defined features.
            It took time to landing this page because I have to learn HTML, CSS, and JavaScript. Quite an achievement!</i></p>
        <p><i>However, there are billions of pages out there, and only small portion gain a glimpse. Myriad of things have to do that make you offer some credit to me.
            Hope that you will enjoy this page. Peace!</i></p>
    </div>
</div>
</div>
<!-- Newest posts -->
<div class="container padding">
<div class="row welcome text-center padding">
    <div class="col-12">
        <h2 class="display-4">Newest posts</h2>
        <ul class="list-group">
            {% for post in site.posts limit:5 %}
            <li class="list-group-item">
                <h3>
                    <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
                </h3>
                <!-- Post truncated -->
                <span class="font-weight-bold">{{ post.date | date: "%b %-d, %Y" }}</span>
                <br>
                <div class="border-top">
                    {{ post.content | strip_html | truncatewords: 20 }}
                    <a href="{{ post.url }}">read more</a>
                </div>
            </li>
            {% endfor %}
        </ul>
    </div>
</div>
</div>
<!-- Welcome section -->
<div class="container-fluid padding">
    <div class="row welcome text-center">
        <div class="col-12">
            <h1 class="display-4">
                Trong-Doan Nguyen
            </h1>
            <hr>
        </div>
        <div class="col-12">
            <p class="lead">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quos iusto officia voluptates rerum minima quas repellat officiis autem, corporis laboriosam praesentium, explicabo debitis ad nesciunt voluptate blanditiis ipsa inventore quaerat esse maxime illo, ex asperiores! Est veritatis temporibus velit itaque?</p>
        </div>
    </div>     
</div>
<!-- Two columns section 1 -->
<div class="container-fluid padding">
    <div class="row padding jumbotron">
        <div class="col-sm-12 col-md-6 col-lg-6">
            <h2>Dynamics &amp; Control</h2>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Libero asperiores a vero corporis itaque dignissimos?</p>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sit laboriosam voluptatibus, tempore veritatis illo eius odio itaque excepturi unde, consequuntur ipsa.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate sunt facere aspernatur, expedita, laudantium natus nihil error quas corporis est amet laborum illo.</p>
            <br>
            <a href="#" class="btn btn-primary">Learn more...</a>
        </div>
        <div class="col-sm-12 col-lg-6 col-md-6">
            <img src="{{site.url}}/images/desk.png" class="img-fluid">
        </div>
    </div>      
</div>

<!-- Two columns section 2 -->
<div class="container-fluid padding">
    <div class="row padding">
        <div class="col-sm-12 col-lg-6 col-md-6">
            <img src="{{site.url}}/images/desk.png" class="img-fluid">
        </div>
        <div class="col-sm-12 col-md-6 col-lg-6">
            <h2>Artificial Intellicence</h2>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Libero asperiores a vero corporis itaque dignissimos?</p>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sit laboriosam voluptatibus, tempore veritatis illo eius odio itaque excepturi unde, consequuntur ipsa.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate sunt facere aspernatur, expedita, laudantium natus nihil error quas corporis est amet laborum illo.</p>
            <br>
            <a href="#" class="btn btn-primary">Learn more...</a>
        </div>

    </div>        
</div>
<!-- Two columns section 3 -->
<div class="container-fluid padding">
    <div class="row padding jumbotron">
        <div class="col-sm-12 col-md-6 col-lg-6">
            <h2>Vlogging</h2>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Libero asperiores a vero corporis itaque dignissimos?</p>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sit laboriosam voluptatibus, tempore veritatis illo eius odio itaque excepturi unde, consequuntur ipsa.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate sunt facere aspernatur, expedita, laudantium natus nihil error quas corporis est amet laborum illo.</p>
            <br>
            <a href="#" class="btn btn-primary">Learn more...</a>
        </div>
        <div class="col-sm-12 col-lg-6 col-md-6">
            <img src="{{site.url}}/images/desk.png" class="img-fluid">
        </div>
    </div>          
</div>
<!-- Connect -->
<div class="container-fluid padding">
    <div class="text-center welcome padding">
        <div class="col-12">
            <h2>Connect</h2>
        </div>
        <hr class="my-4"> 
        <div class="col-12 social padding">
            <a href="https://www.facebook.com/nguyentrongdoan.0"><i class="fab fa-facebook"></i></a>
            <a href="https://www.linkedin.com/in/nguyen-doan-trong/"><i class="fab fa-linkedin"></i></a>
            <a href="https://www.youtube.com/channel/UCaC5rKkxBjV-82_64F9FgcQ"><i class="fab fa-youtube"></i></a>
        </div>
    </div>  
</div>