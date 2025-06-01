<script>
    import Hero from "$lib/Hero.svelte";

    const images = [
        '0983.JPG', 
        'IMG_0469.PNG', 
        'IMG_0470.PNG', 
        'IMG_0513.JPG', 
        'IMG_1451.PNG', 
        'IMG_2530.JPG', 
        'IMG_2872.JPG', 
        'IMG_3751.JPG', 
        'IMG_4993.JPG', 
        'IMG_5393.PNG', 
        'IMG_7288.JPG', 
        'IMG_9774.JPG', 
        'IMG_9897.JPG', 
        'stock', 
        'Waiting.JPG'
    ]
</script>
<Hero>
    <div class="featured-image-container">
    </div>
</Hero>
<Hero section_name="featured">
    <h1 class="featured-header">Featured</h1>
    <div class="grid-container">
        {#each images as image, index}
            <div class={`featured-grid-${index + 1}`} data-grid-index={`${index + 1}`}>
                <img class="featured-grid-image" src={`https://raw.githubusercontent.com/08Aristodemus24/lalais-portfolio/master/client-side/src/assets/mediafiles/${image}`} alt=""/>
            </div>
        {/each}
    </div>
</Hero>
