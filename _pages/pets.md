---
title: Pets
layout: collection   # para el liquid deberia de comentar esta linea
permalink: /pets/
collection: pets
entries_layout: grid
classes: wide
---

Sample document listing for the collection `_pets`.

{% for pet in site.pets %}
    <h2>{{ pet.title }} </h2>   # - {{ pet.position }} 
{% endfor %}


# Aqui iria el liquid