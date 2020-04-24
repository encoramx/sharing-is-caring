---
layout: default
---

<section class="hero">
  <div class="container">
    <div class="row justify-content-center text-center">
      <div class="col-12 col-lg-7 mb-5 mb-lg-0">
        <h1 class="text-orange display-3 font-weight-bold">{{ site.title }}</h1>
        <p class="lead">{{ site.description }}</p>
      </div>
    </div>
  </div>
</section>

<section class="overlap-before pb-0">
  <div class="container pt-5">
    <div class="row align-items-stretch justify-content-center">
      {% for piece in site.data.pieces.list %}
      <div class="col-lg-5 col-md-8 d-flex align-items-stretch">
        <div class="box mb-4 d-flex flex-column">
          <a href="{{ piece.url }}" target="_blank" class="cover"><img src="{{ piece.image }}"
              alt="{{ piece.title }}"></a>
          <div class="px-4 py-4">
            <h2 class="h4 text-orange"><a href="{{ piece.url }}" target="_blank">{{ piece.title }}</a></h2>
            <p class="text-grey">{{ piece.description }}</p>
          </div>
          <div class="bg-light-orange px-4 py-4 text-center mt-auto">
            <p class="mb-0">Share on:&nbsp;
              <a href="https://twitter.com/intent/tweet?url={{ piece.url }}&amp;text={{ piece.title }}%0D%0Avia @nearsoft%0D%0A"
                class="share twitter btn btn-primary"><i class="fa fa-twitter"></i><span> Twitter</span></a>
              <a href="https://www.facebook.com/sharer/sharer.php?u={{ piece.url }}"
                class="share facebook btn btn-primary"><i class="fa fa-facebook"></i><span> Facebook</span></a>
              <a href="https://www.linkedin.com/shareArticle?mini=true&amp;url={{ piece.url }}&amp;title={{ piece.title }}&amp;summary={{ piece.description }}&amp;source="
                class="share linkedin btn btn-primary"><i class="fa fa-linkedin"></i><span> Linkedin</span></a>
            </p>
          </div>
        </div>
      </div>
      {% endfor %}
    </div>
  </div>
</section>


<section class="py-5">
  <div class="container">
    <div class="row justify-content-center text-center">
      <div class="col-lg-6">
        <p class="mb-0">Thanks for your support.</p>
        <p class="mb-0">The Nearsoft Marketing Team</p>
        <p><i class="fa fa-heart text-orange"></i></p>
      </div>
    </div>
  </div>
</section>