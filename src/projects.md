---
layout: page
title: Projects
---

<ul>
  <% collections.projects.resources.each do |project| %>
    <li>
      <a href="<%= project.relative_url %>"><%= project.data.title %></a>
    </li>
  <% end %>
</ul>
