---
layout: page
title: Our Team
permalink: /team/
---

<style>
  .member-image {
    height: 120px;
    width: auto;
    object-fit: cover;
  }

  .team-member {
    margin-bottom: 30px;
  }
</style>

## Meet Our Research Team

{% for member in site.data.team_members %}
<div class="team-member">
  <img src="{{ member.image | relative_url }}" alt="{{ member.name }}" class="member-image">
  <h2>{{ member.name }}</h2>
  <h3>{{ member.title }}</h3>
  <p><strong>Role:</strong> {{ member.role }}</p>
  <p>{{ member.bio }}</p>
</div>
{% endfor %}


## Former Members



