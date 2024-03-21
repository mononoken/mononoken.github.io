---
layout: page
title: Projects
---

<ul>
  <% collections.projects.resources.each do |project| %>
    <li class="project">
      <%= render "project", project: project %>
    </li>
  <% end %>
  <li class="project">
    <div>
      <h1>
        <%= link_to "Many more at Github", "https://github.com/mononoken" %>
      </h1>
    </div>
  </li>
</ul>
