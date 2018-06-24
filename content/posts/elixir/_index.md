<section class="container list">
  <ul>
    {{ range .Paginator.Pages (where .Site.Pages "Section")}}
    <li>
      <span>{{ .Date.Format "January 2, 2006" }}</span><a href="{{ .URL }}">{{ .Title }}</a>
    </li>
    {{ end }}
  </ul>
  {{ partial "pagination.html" . }}
</section>
