---
# generic fallback item page layout 
# displays image or icon depending on "image_thumb"
layout: item/item-page-base
---

<div class="card mb-4 text-center">
    <div class="card-body">
        
       <!-- embeds an IA book reader object for a parent or non-compound object :) -->
{% assign archive_id = page.object_location | split: '/' | last %}
<div class="ratio ratio-4x3" >
    <iframe src="https://archive.org/embed/{{archive_id}}" width="640" height="480" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true" allowfullscreen></iframe>
</div>
        <div class="mt-2">

            {% include item/download-buttons.html %}

        </div>

    </div>
</div>
