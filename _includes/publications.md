<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
    <div class="col-sm-3 abbr" style="position: relative;padding-right: 0px;padding-left: 0px;">
        {% if link.image %} 
        <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
        {% endif %}
        {% if link.conference_short %} 
        <abbr class="badge">{{ link.conference_short }}</abbr>
        {% endif %}
    </div>
    <div class="col-sm-9" style="position: relative;padding-right: 0px;padding-left: 110px;">
        {% if link.tag %}
            <div class="title" id="{{ link.tag }}"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
        {% else %}
            <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
        {% endif %}
        <div class="author">{{ link.authors }}</div>
        <div class="periodical">{{ link.conference }}</div>
        {% if link.notes %} 
            <div> <span>{{ link.notes }}</span></div>
        {% endif %}
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
            {% if link.video %} 
            <a href="{{ link.video }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Video</a>
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

</ol>
</div>

