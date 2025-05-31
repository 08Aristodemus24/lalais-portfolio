<script>
    import Hero from "$lib/Hero.svelte";

    const images = [
        '07def50302447f77b01e4f6804bd3d43_784f979e-61d1-4196-a09f-94139733edb3.png', 
        '1280px-Sacrifice_of_Isaac-Caravaggio_(Uffizi).jpg', 
        '131500.jpg', 
        '1917-movie-4k-ic.jpg', 
        '1937886.jpg', 
        '341844.jpg', 
        '403505.jpg', 
        '59-590186_world-war-2-tank-wallpaper-12378-hd-wallpapers.jpg', 
        '72598-World_War_II-beach-Omaha_Beach-people.jpg', 
        '7ed965a33087a0156722c8815f322a46.jpg', 
        '90c85684c26fc83a166784ea999a7051.jpg', 
        '9AOxoC.jpg', 
        'journey-painting-wallpaper.jpg', 
        'the_wolverine-hd_wallpapers.jpg',
    ]
</script>
<Hero>
    <div class="featured-image-container">
    </div>
</Hero>
<Hero section_name="featured">
    <h1 class="featured-header">featured</h1>
    <div class="featured-grid-container">
        {#each images as image, index}
            <div class={`featured-grid-${index + 1}`} data-grid-index={`${index + 1}`}>
                <img class="featured-grid-image" src={`https://raw.githubusercontent.com/08Aristodemus24/lalais-portfolio/master/client-side/src/assets/mediafiles/${image}`} alt=""/>
            </div>
        {/each}
    </div>
</Hero>
