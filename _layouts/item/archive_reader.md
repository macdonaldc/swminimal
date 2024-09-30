---
# basic video item layout
# Displays a video embedded on the page with default support for video files (using <video> element with object_location as src, MP4 is most compatible format), YouTube (from full link in object_location), or Vimeo videos (from full link in object_location).
layout: item/item-page-base
---

<div class="card mb-4 text-center">
    <div class="card-body">
    
       <!-- embeds an IA book reader object for a parent or non-compound object :) -->
{% assign archive_id = page.object_location | split: '/' | last %}
<div class="ratio ration-4x3">
    <iframe src="https://archive.org/embed/{{ archive_id }}" width="560" height="384" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true" allowfullscreen></iframe>
</div>

        <div class="mt-2">
            
            {% include item/download-buttons.html %}
           
        </div>
        
    </div>
</div>
