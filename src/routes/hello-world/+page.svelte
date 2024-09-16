<script lang="ts">
    import type { PageData } from './$types';
    let message: string = "Hello World";
    export let data: PageData;
</script>

<!-- Bind the message variable to the template for display -->
<h1>{message}</h1>