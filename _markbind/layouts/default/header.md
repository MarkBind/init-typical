<header>
<navbar type="dark">
  <a slot="brand" href="/" title="Home" class="navbar-brand">Your Logo</a>
  <li><a href="{{ baseUrl }}/topics/topic1.html" class="nav-link">Topic 1</a></li>
  <li><a href="{{ baseUrl }}/topics/placeholder.html" class="nav-link">Topic 2</a></li>
  <li><a href="{{ baseUrl }}/topics/placeholder.html" class="nav-link">Topic 3</a></li>
  <dropdown text="Topic 3" class="nav-link">
    <li><a href="{{ baseUrl }}/topics/placeholder.html" class="dropdown-item">Topic 3a</a></li>
    <li><a href="{{ baseUrl }}/topics/placeholder.html" class="dropdown-item">Topic 3b</a></li>
  </dropdown>
  <li><a href="{{ baseUrl }}/topics/placeholder.html" class="nav-link">Topic 4</a></li>
  <li slot="right">
    <form class="navbar-form">
      <searchbar :data="searchData" placeholder="Search" :on-hit="searchCallback"></searchbar>
    </form>
  </li>
</navbar>
</header>