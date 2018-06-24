<section class="container list">
  <h1 class="title"><a href="/categories/solidity/"><img src="/images/solidity.jpg" height="100" width="100"></a> Solidity Posts</h1>
  <ul>
    {{ range .Paginator.Pages (where .Site.Pages "Section")}}
    <li>
      <span>{{ .Date.Format "January 2, 2006" }}</span><a href="{{ .URL }}">{{ .Title }}</a>
    </li>
    {{ end }}
  </ul>
  {{ partial "pagination.html" . }}
</section>
