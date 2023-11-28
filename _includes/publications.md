<h1 id="publications"></h1>

<h2 style="margin: 60px 0px -15px;">Publications <temp style="font-size:15px;">[</temp><a href="https://scholar.google.com/" target="_blank" style="font-size:15px;">Google Scholar</a><temp style="font-size:15px;">]</temp><temp style="font-size:15px;">[</temp><a href="https://www.researchgate.net/profile/Xinyue-Wang-148" target="_blank" style="font-size:15px;">ResearchGate</a><temp style="font-size:15px;">]</temp></h2>


<div class="publications">
<ol class="bibliography">

<div style="display: none;">
{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
            <abbr class="badge">{{ link.conference_short }}</abbr>
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

<br>

{% endfor %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="" class="teaser img-fluid z-depth-1">
            <abbr class="badge"></abbr>
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="</a></div>
      <div class="author">, <strong></strong>, <br> (* Equal contribution)</div>
      <div class="periodical"><em> <strong></strong></em>
      </div>
    <div class="links">
      <a href="" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;"></a>
      <a href="" role="button" target="_blank" style="font-size:12px;"></a>
      <a href="" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;"></a>
      <a href="https://dblp.uni-trier.de/rec/conf/cvpr/SunLCS19.html?view=bibtex" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
<br>
<strong> <a style="color:#e74d3c; font-weight:600" href="">800+</i><i style="color:#e74d3c; font-weight:600"> Citations • </i></a><a href="" target="_blank" rel="noopener"><i style="color:#e74d3c; font-weight:600" id="githubstars_mtl">600+</i><i style="color:#e74d3c; font-weight:600"> GitHub Stars</i></a> <a style="color:#e74d3c; font-weight:600" href="">• <i></i></a></strong>
<br>
<strong><a style="color:#e74d3c; font-weight:600" href=""><i></i></a></strong>
  <script>
  githubStars("", function(stars) {
  var startext = document.getElementById("githubstars_mtl");
        startext.innerHTML=stars;
  });
  </script>
  <script>
      $(document).ready(function () {
          
          var gsDataBaseUrl = ''
          
          $.getJSON(gsDataBaseUrl + "google-scholar-stats/gs_data.json", function (data) {
              var totalCitation = data['publications']['J:']['num_citations']
              document.getElementById('total_citation_mtl').innerHTML = totalCitation;
              var citationEles = document.getElementsByClassName('show_paper_citations')
              Array.prototype.forEach.call(citationEles, element => {
                  var paperId = element.getAttribute('data')
                  var numCitations = data['publications'][paperId]['num_citations']
                  element.innerHTML = '| Citations: ' + numCitations;
              });
          });
      })
  </script>
    </div>
  </div>
</div>
</li>

</ol>
</div>


