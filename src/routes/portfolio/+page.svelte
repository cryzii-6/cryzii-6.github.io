<script>
  let images = [
    '/images/1.jpg',
    '/images/2.jpg',
    '/images/3.jpg',
    '/images/4.jpg',
    '/images/5.jpg',
    '/images/6.jpg',
  ];
</script>

<main class="p-4">
  <h1 class="text-3xl font-bold text-center mb-6">Ynnyannah's Gallery</h1>
  <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4">
    {#each images as image}
      <div class="overflow-hidden rounded-lg shadow-lg">
        <img src={image} alt="Gallery Image" class="w-full h-full object-cover transition-transform duration-200 transform hover:scale-105" />
      </div>
    {/each}
  </div>
</main>

<style>
  img {
    filter: brightness(0.9);
  }
  main {
    background-color: rgb(23, 142, 221); 
  }
</style>
