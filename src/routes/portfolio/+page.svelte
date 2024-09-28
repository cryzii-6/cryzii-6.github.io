<script>
  let images = [
    '/images/1.jpg',
    '/images/2.jpg',
    '/images/3.jpg',
    '/images/4.jpg',
    '/images/5.jpg',
    '/images/6.jpg',
    '/images/7.jpg',
    '/images/8.jpg',
    '/images/9.jpg',
    '/images/10.jpg',
    '/images/11.jpg',
    '/images/12.jpg',
  ];

  /**
     * @type {string | null}
     */
  let selectedImage = null; // To store the clicked image

  // Function to close the modal
  function closeModal() {
    selectedImage = null;
  }
</script>

<main class="p-4">
  <h1 class="text-3xl font-bold text-center mb-6">Ynnyannah's Gallery</h1>
  <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4">
    {#each images as image}
      <div class="overflow-hidden rounded-lg shadow-lg">
        <img 
          src={image} 
          alt="Gallery Image" 
          class="w-full h-full object-cover transition-transform duration-200 transform hover:scale-105 cursor-pointer"
          on:click={() => selectedImage = image} />
      </div>
    {/each}
  </div>

  {#if selectedImage}
    <div class="modal" on:click={closeModal}>
      <div class="modal-content">
        <img src={selectedImage} alt="Selected Image" />
      </div>
    </div>
  {/if}
</main>

<style>
  img {
    filter: brightness(0.9);
  }

  main {
    background-color: rgb(23, 142, 221); 
  }

  /* Modal Styles */
  .modal {
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    background-color: rgba(0, 0, 0, 0.8);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 10;
    cursor: pointer;
  }

  .modal-content {
    max-width: 90%;
    max-height: 90%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .modal-content img {
    width: auto;
    height: auto;
    max-width: 100%;
    max-height: 100%;
    border-radius: 12px;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
  }

  /* For responsive design */
  @media (max-width: 600px) {
    .modal-content img {
      width: 100%;
    }
  }
</style>
