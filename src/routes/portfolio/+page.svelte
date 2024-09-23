<script>
  let images = [
    'https://scontent.fmnl9-6.fna.fbcdn.net/v/t39.30808-6/461108675_2765528513610413_4849604239128053632_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeF4ENUuQToqLUEUbWhvgSPgsVqpEo24mWuxWqkSjbiZa01JZF0W1bCt5fegsSLoP7L0ldww97kq_MXIVLV1bkWV&_nc_ohc=sPx6vLf3Y6kQ7kNvgFB9Czn&_nc_ht=scontent.fmnl9-6.fna&oh=00_AYD3uiDYIfeEHY5Hsll2l1Hx9GJYzbV2_jOATMZpUboZIA&oe=66F6F267',
    'https://scontent.fmnl9-6.fna.fbcdn.net/v/t39.30808-6/461206819_2765529393610325_4877227520079747330_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeGp4iVY9Ic6KOHLRTGBPV0ylatlNeDYxlWVq2U14NjGVS3DwHj0jc-egvbLsiEkS3bNUZn1mNGx4WmGq-2PWcC6&_nc_ohc=2X_bSYKnbgIQ7kNvgG9yp_h&_nc_ht=scontent.fmnl9-6.fna&_nc_gid=A1tErtcSP-QtL8LmKErQznG&oh=00_AYDi6Ig_J9kNoImnTA-oT6-OcKBZxgCZqKH0Bct31Xe9bg&oe=66F704E7',
    'https://scontent.fmnl9-4.fna.fbcdn.net/v/t39.30808-6/460989813_2765529463610318_7779405720491128306_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeELscOnydoG5Faw6b_1CueXwzdwXeSZw_3DN3Bd5JnD_Q84N23sNfGK_WfWVMWXIRm-XO-zo5wN8xr8ufoGqhxF&_nc_ohc=JvyrT8EgQygQ7kNvgGJI8ep&_nc_ht=scontent.fmnl9-4.fna&oh=00_AYCAdRE0q3-QCy6r91x6qhVyNVTaJ0xqpzgN4Pvz1zd6Sg&oe=66F72264',
    'https://scontent.fmnl9-3.fna.fbcdn.net/v/t39.30808-6/461109964_2765529696943628_3282180731821659130_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeE-mAInm9aWYzWPl4LWZTuflV-wsswpLOqVX7CyzCks6ssw6QskXndK7GDxiYtyNx4H6yKt73ieu9w03Q-rejWq&_nc_ohc=7cnTfopKGrkQ7kNvgE5F8CZ&_nc_ht=scontent.fmnl9-3.fna&_nc_gid=AoEl-IO1Mq_bgISj3l44oqr&oh=00_AYA4wujDhUW88zLLHen8vVD3uiuGrQbH4YrhM_FxA6tRRA&oe=66F6F3A6',
    'https://scontent.fmnl9-6.fna.fbcdn.net/v/t39.30808-6/461061290_2765532610276670_2545279684488805240_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeGLt6nrqTNnjDlBA08_IaYpZDqe8Qn7u51kOp7xCfu7nS6Sg1aZ8jBHsUd-I9vDxNq-3yBVF2LVFdtYOVaWAc8-&_nc_ohc=74kGP5ZYBcsQ7kNvgFff8U-&_nc_ht=scontent.fmnl9-6.fna&_nc_gid=AWbqtgNWJj-F6obAYrHl2zx&oh=00_AYCAyGRB2nqf-zyC4XrYmWjPRRD2ECsOl0yFn8s7SJl1Nw&oe=66F6F5D3',
    'https://scontent.fmnl9-4.fna.fbcdn.net/v/t39.30808-6/461177472_2765535053609759_663404577154438806_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeFB0O7H_ZXems_OjTsKjUQWIH7zjazQV0EgfvONrNBXQXh2tmZunnf53WnY-HYfkPjmFfLaxJkbiJm5pzaJDC8H&_nc_ohc=wrGg-o0J-7AQ7kNvgHxUSj0&_nc_ht=scontent.fmnl9-4.fna&_nc_gid=A21DQL9pBOstFt_6lqc2_ug&oh=00_AYD9uDWAXXWIBv_nKOXkSTrKjowFKO_LjUlOzGLr9U_1Ng&oe=66F71A46',
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


