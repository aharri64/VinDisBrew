# VinDisBrew

This applicaton is not yet complete.

> **Please check the Planning folder for more information**

'''

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Authentication</title>
    <link rel="stylesheet" href="/css/style.css">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-BmbxuPwQa2lc/FVzBcNJ7UAyJxM6wuqIj61tLrc4wSX0szH/Ev+nYRRuWlolflfl" crossorigin="anonymous">
  </head>
  <body>
    <%- include('partials/alerts') %>
    <header>
      <nav>
        <ul>
          <% if (!currentUser) {%>
          <li><a href="/auth/signup">Signup</a></li>
          <li><a href="/auth/login">Login</a></li>
          <% } else { %>
          <li><a href="/auth/logout">Logout</a></li>
          <li><a href="/profile">Profile</a></li>
          <% } %> 
        </ul>
      </nav>
    </header>
    <h1>Authentication</h1>
    <%- body %>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta2/dist/js/bootstrap.bundle.min.js" integrity="sha384-b5kHyXgcpbZJO/tY9Ul7kGkf1S0CWuKcCD38l8YkeH8z8QjE0GmW1gYU5S9FOnJ0" crossorigin="anonymous"></script>
  </body>
</html>
'''
