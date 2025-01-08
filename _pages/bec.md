---
title: "EQCOS"
layout: textwithmath
excerpt: "EQCOS"
sitemap: false
permalink: /bec/
---


# EQCOS















 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi et ultrices turpis, ut volutpat ipsum. Integer commodo tellus id est tempor ornare. Donec felis tortor, malesuada in vestibulum at, dapibus et magna. Donec et vestibulum libero. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent et dapibus nibh, eget laoreet libero. Integer eu odio ac ante ornare porttitor quis in felis. Praesent placerat quam vel tortor bibendum vehicula. Duis id ante pretium, lacinia elit ac, volutpat arcu.

Praesent egestas dapibus urna, auctor blandit odio ultricies sit amet. Aliquam feugiat pellentesque ante. Aliquam a finibus orci, sed luctus ex. Nam ut ligula ut metus pharetra hendrerit at sit amet eros. Fusce fermentum laoreet nibh at semper. Suspendisse vehicula, eros non sodales volutpat, metus nisi elementum mi, in faucibus ex odio nec velit. Sed rutrum tortor commodo nulla laoreet, eget egestas est luctus. Nullam sed neque sit amet sem tincidunt faucibus accumsan egestas augue. Donec vehicula urna dapibus risus efficitur dictum.

Mauris eu rhoncus neque, a convallis lacus. Vivamus lobortis enim orci, sit amet rutrum dui pretium quis. Praesent ante ipsum, ultricies sed dui et, vestibulum posuere purus. Mauris vel nibh quis tortor tempor consequat in in nunc. Nunc rutrum turpis diam, ut maximus quam ultricies eget. Curabitur condimentum ultrices massa, non porta dui posuere quis. Donec sit amet libero enim.  </b>


<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="5000" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        {% assign slide_number = 0 %}
        {% for image in site.data.bec-carousel %}
        {% if slide_number == 0 %}
            <li data-target="#carousel" data-slide-to="{{ slide_number }}" class="active"></li>
        {% else %}
        <li data-target="#carousel" data-slide-to="{{ slide_number }}"></li>
        {% endif %}
        {% assign slide_number = slide_number | plus: 1 %}
        {% endfor %}
    </ol>
    <!-- Items -->
    <div class="carousel-inner" markdown="0">
    {% assign slide_number = 0 %}
    {% for image in site.data.bec-carousel %}

        {% if slide_number == 0 %}
            <div class="item active">
        {% else %}
            <div class="item">
        {% endif %}
            <img src="{{ site.url }}{{ site.baseurl }}/images/{{ image.image }}" alt="Slide {{ slide_number }}" />
        </div>

    {% assign slide_number = slide_number | plus: 1 %}
    {% endfor %}
    </div>
  <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>







