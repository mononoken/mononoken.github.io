---
layout: page
title: Posts
---

<ul>
  <% collections.posts.resources.each do |post| %>
    <li>
      <span><%= post.data.date.strftime("%Y-%m-%d") %> </span><a href="<%= post.relative_url %>"><%= post.data.title %></a>
    </li>
  <% end %>
</ul>
