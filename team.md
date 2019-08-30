---
layout: default
title: L'équipe SchoolMouv
---

<div id="team">
  <h1>L'équipe</h1>
  <ul class="posts noList listing">
    {% for member in site.data.team %}
      <li class="team-member">
        <div>
          <img src="{{ '/assets/img/team/'| append: member.photo | prepend: site.baseurl }}" alt="photo"/>
        </div>
        <div>
          <h3>{{ member.name }}</h3>
          <span class="date">{{ member.job }}</span>
        </div>
      </li>
    {% endfor %}
  </ul>
</div>

<style>

#team .posts li::before {
  content: none;
}

#team .listing {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  margin-top: 40px;
}

#team .team-member {
  display: flex ;
  flex-direction: row ;
  width: 50%;
}

#team .team-member h3 {
  font-size: 1.2em;
}

#team .team-member img {
  margin: 0 20px ;
}

@media (max-width: 1200px) {
  #team .team-member {
    width: 100%;
  }
}
</style>
