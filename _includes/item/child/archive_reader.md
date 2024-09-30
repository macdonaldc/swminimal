`<!-- embeds an IA book reader object for a parent or non-compound object :) -->
{% assign archive_id = page.object_location | split: '/' | last %}
<div class="ratio ratio-4x3" >
    <iframe src="https://archive.org/embed/{{ archive_id }}" width="560" height="384" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true" allowfullscreen></iframe>
</div>`