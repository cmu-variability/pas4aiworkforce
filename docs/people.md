---
title: People
hide:
    - navigation
---

## Principal Investigators

<div id="PIs">
{%- set pis = extra.people | selectattr("role", "==", "PI") | list -%}
{% for pi in pis %}
<div class="pi card">
    <div class="container">
        <img class="pi-image" src="../assets/images/{{pi.photo}}" alt="">
        <div>
            <h3 class="pi-name">
                {% if pi.website %}
                    <a href="{{pi.website}}" target="_blank">
                        {{pi.name}}
                    </a>
                {% else %}
                    {{pi.name}}
                {% endif %}
            </h3>
            <div class="pi-bio">
                {{pi.bio}}
            </div>
            {% if pi.affiliation %}
                <div class="pi-affiliation">{{pi.affiliation}}</div>
		    {% endif %}
        </div>
    </div>
</div>
{% endfor %}
</div>

## Senior Personnel

<div id="PIs">
{%- set pis = extra.people | selectattr("role", "==", "Senior") | list -%}
{% for pi in pis %}
<div class="pi card">
    <div class="container">
        <img class="pi-image" src="../assets/images/{{pi.photo}}" alt="">
        <div>
            <h3 class="pi-name">
                {% if pi.website %}
                    <a href="{{pi.website}}" target="_blank">
                        {{pi.name}}
                    </a>
                {% else %}
                    {{pi.name}}
                {% endif %}
            </h3>
            <div class="pi-bio">
                {{pi.bio}}
            </div>
            {% if pi.affiliation %}
                <div class="pi-affiliation">{{pi.affiliation}}</div>
		    {% endif %}
        </div>
    </div>
</div>
{% endfor %}
</div>

## External Evaluator

<div id="PIs">
{%- set pis = extra.people | selectattr("role", "==", "Evaluator") | list -%}
{% for pi in pis %}
<div class="pi card">
    <div class="container">
        <img class="pi-image" src="../assets/images/{{pi.photo}}" alt="">
        <div>
            <h3 class="pi-name">
                {% if pi.website %}
                    <a href="{{pi.website}}" target="_blank">
                        {{pi.name}}
                    </a>
                {% else %}
                    {{pi.name}}
                {% endif %}
            </h3>
            <div class="pi-bio">
                {{pi.bio}}
            </div>
            {% if pi.affiliation %}
                <div class="pi-affiliation">{{pi.affiliation}}</div>
		    {% endif %}
        </div>
    </div>
</div>
{% endfor %}

</div>
