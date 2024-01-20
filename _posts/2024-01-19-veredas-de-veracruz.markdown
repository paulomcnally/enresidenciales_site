---
layout: post
title:  "Veredas de Veracruz"
date:   2024-01-19 19:39:23 -0600
categories: veredas-de-veracrus
permalink: /ni/veredas-de-veracruz/
services:
-
  title: Aguja y Seguridad - El Emperador S.A. 1
  name: Seguridad
  description: Acceso y seguridad del residencial.
  phone_number: +505 57025414
  image: guarda.png
-
  title: Aguja y Seguridad - El Emperador S.A. 2
  name: Seguridad
  description: Acceso y seguridad del residencial.
  phone_number: +505 85709484
  image: guarda.png
-
  title: Gas y Agua Express
  name: Agua
  description: Agua pura - Fuente pura.
  phone_number: +505 8321 4021
  image: agua.png
-
  title: Gas y Agua Express
  name: Gas
  description: Gas butano - Tropigas.
  phone_number: +505 8321 4021
  image: gas.png
---
 {% for service in page.services %}
<div class="card bg-light-subtle mt-4">
    <img src="/assets/images/{{ service.image }}" class="card-img-top" alt="{{ service.title }}">
    <div class="card-body">
      <div class="text-section">
        <h5 class="card-title">{{ service.title }}</h5>
        <p class="card-text">{{ service.description }}</p>
      </div>
      <div class="cta-section">
        <div>{{ service.name }}</div>
        <a href="tel:{{ service.phone_number }}" class="btn btn-light">Llamar</a>
      </div>
    </div>
  </div>
{% endfor %}