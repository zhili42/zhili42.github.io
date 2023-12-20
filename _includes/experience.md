<h2 id="experience">Industry Experience</h2>

<div class="experiences">
<ol class="bibliography">

{% for exp in site.data.experience.main %}

<li>
<div class="exp-row">
    <div class="col-sm-3" style="position: relative;padding-right: 0px;padding-left: 0px;">
        {% if exp.company_logo %} 
        <img src="{{ exp.company_logo }}" width="200px">
        {% endif %}
    </div>
    <div class="col-sm-9" style="position: relative;padding-right: 0px;padding-left: 20px;">
            <div> <b>{{ exp.title }}</b>, <b>{{ exp.company }}</b>, {{ exp.location }}</div>
            <div>{{ exp.time }}</div>
            <div>{{ exp.job }}</div>
    </div>
</div>
</li>

{% endfor %}

</ol>
</div>

