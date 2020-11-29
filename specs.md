---
layout: default
title: Specifications
---
{%- include variables.html -%}
<div class="row">
    {% for api in site.apis %}
    <div class="col-lg-4">
            <div class="card bg-secondary mb-3" style="max-width: 20rem;">
              <div class="card-header"><i class="fa {{api.icon}} px-lg-2" aria-hidden="true"></i>{{api.title}}</div>
              <div class="card-body">
                <h4 class="card-title">Version: {{api.version}}</h4>
                <p class="card-text">{{api.description}}</p>
                <a href="{{api.url}}" class="btn btn-secondary">{{dictionary.generateAPIDoc}}</a>
              </div>
        </div>
    </div>
    {% endfor %}
</div>