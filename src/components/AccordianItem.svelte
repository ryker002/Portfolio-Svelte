<script>
    export let id;
    export let title;
    export let content;
    export let parent;
</script>

<style>
    .accordion-button {
        font-family: effra;
        text-transform: uppercase;
        font-weight: 200;
    }
    .accordion-body {
        color: #000;
        font-family: effra;
    }
</style>

<div class="accordion-item">
    <h2 class="accordion-header" id={id}>
    <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#{id}-target" aria-expanded="false" aria-controls="flush-collapseOne">
        {title}
    </button>
    </h2>
    <div id="{id}-target" class="accordion-collapse collapse" aria-labelledby="careers-headingOne" data-bs-parent="#{parent}">
    <div class="accordion-body">{content}</div>
    </div>
</div>